# Schemas: blanketPurchaseOrder

Property tables for definitions owned by `blanketPurchaseOrder`.

Record page: [blanketPurchaseOrder](../records/blanketPurchaseOrder.md).

## Index

- [blanketPurchaseOrder](#blanketpurchaseorder) — 72 properties
- [blanketPurchaseOrder-accountingBookDetailCollection](#blanketpurchaseorder-accountingbookdetailcollection) — 6 properties
- [blanketPurchaseOrder-accountingBookDetailElement](#blanketpurchaseorder-accountingbookdetailelement) — 7 properties
- [blanketPurchaseOrder-expense-orderSchedule](#blanketpurchaseorder-expense-orderschedule) — 27 properties
- [blanketPurchaseOrder-expense-orderSchedule-scheduleCollection](#blanketpurchaseorder-expense-orderschedule-schedulecollection) — 6 properties
- [blanketPurchaseOrder-expense-orderSchedule-scheduleElement](#blanketpurchaseorder-expense-orderschedule-scheduleelement) — 10 properties
- [blanketPurchaseOrder-expenseCollection](#blanketpurchaseorder-expensecollection) — 6 properties
- [blanketPurchaseOrder-expenseElement](#blanketpurchaseorder-expenseelement) — 15 properties
- [blanketPurchaseOrder-item-orderSchedule](#blanketpurchaseorder-item-orderschedule) — 27 properties
- [blanketPurchaseOrder-item-orderSchedule-scheduleCollection](#blanketpurchaseorder-item-orderschedule-schedulecollection) — 6 properties
- [blanketPurchaseOrder-item-orderSchedule-scheduleElement](#blanketpurchaseorder-item-orderschedule-scheduleelement) — 11 properties
- [blanketPurchaseOrder-itemCollection](#blanketpurchaseorder-itemcollection) — 6 properties
- [blanketPurchaseOrder-itemElement](#blanketpurchaseorder-itemelement) — 46 properties
- [blanketPurchaseOrderCollection](#blanketpurchaseordercollection) — 6 properties
- [blanketPurchaseOrderSelectOptions](#blanketpurchaseorderselectoptions) — 20 properties

## blanketPurchaseOrder

Browser definition `blanketPurchaseOrder`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBookDetail` |  | blanketPurchaseOrder-accountingBookDetailCollection |  |  | [`blanketPurchaseOrder-accountingBookDetailCollection`](#blanketpurchaseorder-accountingbookdetailcollection) |  |
| `approvalStatus` |  | object |  |  |  |  |
| `approvalStatus.id` | Internal identifier | string |  |  |  | `11`, `1`, `2`, `3` |
| `approvalStatus.refName` | Reference Name | string |  |  |  |  |
| `billedAmount` | Billed Amount | number | double |  |  |  |
| `billingInstructions` | Billing Instructions | string |  |  |  |  |
| `carrier` | Carrier | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
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
| `excludefromsupplyplanning` | Exclude from Supply Planning | boolean |  |  |  |  |
| `expense` |  | blanketPurchaseOrder-expenseCollection |  |  | [`blanketPurchaseOrder-expenseCollection`](#blanketpurchaseorder-expensecollection) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `incoTerm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `item` |  | blanketPurchaseOrder-itemCollection |  |  | [`blanketPurchaseOrder-itemCollection`](#blanketpurchaseorder-itemcollection) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `maximumAmount` | Maximum Amount | number | double |  |  |  |
| `memo` | Memo | string |  |  |  |  |
| `message` | Vendor Message | string |  |  |  |  |
| `nextApprover` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `orderStatus` |  | object |  |  |  |  |
| `orderStatus.id` | Internal identifier | string |  |  |  | `A`, `R`, `B`, `H` |
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
| `status.id` | Internal identifier | string |  |  |  | `A`, `R`, `B`, `H` |
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
| `webSite` |  | string |  |  |  |  |

## blanketPurchaseOrder-accountingBookDetailCollection

Browser definition `blanketPurchaseOrder-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | blanketPurchaseOrder-accountingBookDetailElement[] |  |  | [`blanketPurchaseOrder-accountingBookDetailElement`](#blanketpurchaseorder-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## blanketPurchaseOrder-accountingBookDetailElement

Browser definition `blanketPurchaseOrder-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## blanketPurchaseOrder-expense-orderSchedule

Browser definition `blanketPurchaseOrder-expense-orderSchedule`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `createPurchaseOrder` |  | object |  |  |  |  |
| `createPurchaseOrder.id` | Internal identifier | string |  |  |  | `MANUAL`, `LEAD` |
| `createPurchaseOrder.refName` | Reference Name | string |  |  |  |  |
| `createSchedule` |  | object |  |  |  |  |
| `createSchedule.id` | Internal identifier | string |  |  |  | `MANUAL`, `AUTO` |
| `createSchedule.refName` | Reference Name | string |  |  |  |  |
| `currencyPrecision` |  | integer | int64 |  |  |  |
| `endDate` | End Date | string | date |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `item` |  | integer | int64 |  |  |  |
| `lineId` |  | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `maxDate` |  | string | date |  |  |  |
| `maxOrderDate` |  | string | date |  |  |  |
| `minDate` |  | string | date |  |  |  |
| `minOrderDate` |  | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `releaseFrequency` |  | object |  |  |  |  |
| `releaseFrequency.id` | Internal identifier | string |  |  |  | `WEEKLY`, `QUARTERLY`, `DAILY`, `MONTHLY` |
| `releaseFrequency.refName` | Reference Name | string |  |  |  |  |
| `schedule` |  | blanketPurchaseOrder-expense-orderSchedule-scheduleCollection |  |  | [`blanketPurchaseOrder-expense-orderSchedule-scheduleCollection`](#blanketpurchaseorder-expense-orderschedule-schedulecollection) |  |
| `startDate` | Start Date | string | date |  |  |  |
| `total` | Total Amount | number | double |  |  |  |
| `totalScheduled` |  | number | float |  |  |  |
| `transactionId` | Transaction ID | integer | int64 |  |  |  |
| `updateAmount` |  | number | float |  |  |  |
| `updateDays` |  | string |  |  |  |  |

## blanketPurchaseOrder-expense-orderSchedule-scheduleCollection

Browser definition `blanketPurchaseOrder-expense-orderSchedule-scheduleCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | blanketPurchaseOrder-expense-orderSchedule-scheduleElement[] |  |  | [`blanketPurchaseOrder-expense-orderSchedule-scheduleElement`](#blanketpurchaseorder-expense-orderschedule-scheduleelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## blanketPurchaseOrder-expense-orderSchedule-scheduleElement

Browser definition `blanketPurchaseOrder-expense-orderSchedule-scheduleElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `memo` | Memo | string |  |  |  |  |
| `orderSchedule` | Order Schedule | integer | int64 |  |  |  |
| `purchaseOrder` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `quantity` |  | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `release` | Release | boolean |  |  |  |  |
| `tranDate` | Date | string | date |  |  |  |

## blanketPurchaseOrder-expenseCollection

Browser definition `blanketPurchaseOrder-expenseCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | blanketPurchaseOrder-expenseElement[] |  |  | [`blanketPurchaseOrder-expenseElement`](#blanketpurchaseorder-expenseelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## blanketPurchaseOrder-expenseElement

Browser definition `blanketPurchaseOrder-expenseElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `amount` | Amount | number | double |  |  |  |
| `amountOrdered` | Amount Ordered | number | double |  |  |  |
| `baseGrossAmt` | Gross Amount | number | double |  |  |  |
| `category` |  | expenseCategory |  |  | [`expenseCategory`](expenseCategory.md#expensecategory) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `grossAmt` | Gross Amount | number | double |  |  |  |
| `line` | Line | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `orderSchedule` |  | blanketPurchaseOrder-expense-orderSchedule |  |  | [`blanketPurchaseOrder-expense-orderSchedule`](#blanketpurchaseorder-expense-orderschedule) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `taxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## blanketPurchaseOrder-item-orderSchedule

Browser definition `blanketPurchaseOrder-item-orderSchedule`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `createPurchaseOrder` |  | object |  |  |  |  |
| `createPurchaseOrder.id` | Internal identifier | string |  |  |  | `MANUAL`, `LEAD` |
| `createPurchaseOrder.refName` | Reference Name | string |  |  |  |  |
| `createSchedule` |  | object |  |  |  |  |
| `createSchedule.id` | Internal identifier | string |  |  |  | `MANUAL`, `AUTO` |
| `createSchedule.refName` | Reference Name | string |  |  |  |  |
| `currencyPrecision` |  | integer | int64 |  |  |  |
| `endDate` | End Date | string | date |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `item` |  | integer | int64 |  |  |  |
| `lineId` |  | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `maxDate` |  | string | date |  |  |  |
| `maxOrderDate` |  | string | date |  |  |  |
| `minDate` |  | string | date |  |  |  |
| `minOrderDate` |  | string | date |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `releaseFrequency` |  | object |  |  |  |  |
| `releaseFrequency.id` | Internal identifier | string |  |  |  | `WEEKLY`, `QUARTERLY`, `DAILY`, `MONTHLY` |
| `releaseFrequency.refName` | Reference Name | string |  |  |  |  |
| `schedule` |  | blanketPurchaseOrder-item-orderSchedule-scheduleCollection |  |  | [`blanketPurchaseOrder-item-orderSchedule-scheduleCollection`](#blanketpurchaseorder-item-orderschedule-schedulecollection) |  |
| `startDate` | Start Date | string | date |  |  |  |
| `total` | Total Quantity | number | float |  |  |  |
| `totalScheduled` |  | number | float |  |  |  |
| `transactionId` | Transaction ID | integer | int64 |  |  |  |
| `updateAmount` |  | number | float |  |  |  |
| `updateDays` |  | string |  |  |  |  |

## blanketPurchaseOrder-item-orderSchedule-scheduleCollection

Browser definition `blanketPurchaseOrder-item-orderSchedule-scheduleCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | blanketPurchaseOrder-item-orderSchedule-scheduleElement[] |  |  | [`blanketPurchaseOrder-item-orderSchedule-scheduleElement`](#blanketpurchaseorder-item-orderschedule-scheduleelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## blanketPurchaseOrder-item-orderSchedule-scheduleElement

Browser definition `blanketPurchaseOrder-item-orderSchedule-scheduleElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `allocatedDemand` | Allocated Demand | number | float |  |  |  |
| `amount` |  | number | double |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `memo` | Memo | string |  |  |  |  |
| `orderSchedule` | Order Schedule | integer | int64 |  |  |  |
| `purchaseOrder` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `release` | Release | boolean |  |  |  |  |
| `tranDate` | Date | string | date |  |  |  |

## blanketPurchaseOrder-itemCollection

Browser definition `blanketPurchaseOrder-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | blanketPurchaseOrder-itemElement[] |  |  | [`blanketPurchaseOrder-itemElement`](#blanketpurchaseorder-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## blanketPurchaseOrder-itemElement

Browser definition `blanketPurchaseOrder-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `baseGrossAmt` | Gross Amount | number | double |  |  |  |
| `billVarianceStatus` |  | object |  |  |  |  |
| `billVarianceStatus.id` | Internal identifier | string |  |  |  | `NOVARIANCES`, `JOURNALNOTPOSTED`, `JOURNALPOSTED` |
| `billVarianceStatus.refName` | Reference Name | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `grossAmt` | Gross Amount | number | double |  |  |  |
| `initOqpBucket` | Initial OQP Bucket | string |  |  |  |  |
| `isClosed` | Closed | boolean |  |  |  |  |
| `isOpen` | Is Opened | boolean |  |  |  |  |
| `isTaxable` | Taxable | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemSubtype` |  | object |  |  |  |  |
| `itemSubtype.id` | Internal identifier | string |  |  |  | `Sale`, `Purchase`, `Resale` |
| `itemSubtype.refName` | Reference Name | string |  |  |  |  |
| `itemType` |  | object |  |  |  |  |
| `itemType.id` | Internal identifier | string |  |  |  | `Group`, `Description`, `Discount`, `EndGroup`, `GiftCert`, `Subtotal`, `Service`, `ShipItem`, `TaxItem`, `InvtPart`, `Payment`, `Expense`, `NonInvtPart`, `TaxGroup`, `Kit`, `Markup`, `DwnLdItem`, `OthCharge`, `Assembly`, `SubscriPlan` |
| `itemType.refName` | Reference Name | string |  |  |  |  |
| `job` |  | job |  |  | [`job`](job.md#job) |  |
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
| `orderSchedule` |  | blanketPurchaseOrder-item-orderSchedule |  |  | [`blanketPurchaseOrder-item-orderSchedule`](#blanketpurchaseorder-item-orderschedule) |  |
| `printItems` | Print Items | boolean |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityOrdered` | Quantity Ordered | number | float |  |  |  |
| `rate` | Rate | number | double |  |  |  |
| `rateIncludingTax` | Rate | number | double |  |  |  |
| `rateSchedule` | Rate Schedule | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tax1Amt` | Tax Amount | number | double |  |  |  |
| `taxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxRate1` | Tax Rate | number | double |  |  |  |
| `taxRate2` | PST | number | double |  |  |  |
| `units` | Units | string |  |  |  |  |
| `vendorName` | Vendor Name | string |  |  |  |  |

## blanketPurchaseOrderCollection

Browser definition `blanketPurchaseOrderCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | blanketPurchaseOrder[] |  |  | [`blanketPurchaseOrder`](#blanketpurchaseorder) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## blanketPurchaseOrderSelectOptions

Browser definition `blanketPurchaseOrderSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `approvalStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
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

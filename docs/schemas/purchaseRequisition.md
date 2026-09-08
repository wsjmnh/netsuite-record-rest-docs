# Schemas: purchaseRequisition

Property tables for definitions owned by `purchaseRequisition`.

Record page: [purchaseRequisition](../records/purchaseRequisition.md).

## Index

- [purchaseRequisition](#purchaserequisition) — 57 properties
- [purchaseRequisition-accountingBookDetailCollection](#purchaserequisition-accountingbookdetailcollection) — 6 properties
- [purchaseRequisition-accountingBookDetailElement](#purchaserequisition-accountingbookdetailelement) — 7 properties
- [purchaseRequisition-expenseCollection](#purchaserequisition-expensecollection) — 6 properties
- [purchaseRequisition-expenseElement](#purchaserequisition-expenseelement) — 18 properties
- [purchaseRequisition-item-inventoryDetail](#purchaserequisition-item-inventorydetail) — 11 properties
- [purchaseRequisition-item-inventoryDetail-inventoryAssignmentCollection](#purchaserequisition-item-inventorydetail-inventoryassignmentcollection) — 6 properties
- [purchaseRequisition-item-inventoryDetail-inventoryAssignmentElement](#purchaserequisition-item-inventorydetail-inventoryassignmentelement) — 17 properties
- [purchaseRequisition-itemCollection](#purchaserequisition-itemcollection) — 6 properties
- [purchaseRequisition-itemElement](#purchaserequisition-itemelement) — 66 properties
- [purchaseRequisitionCollection](#purchaserequisitioncollection) — 6 properties
- [purchaseRequisitionSelectOptions](#purchaserequisitionselectoptions) — 16 properties

## purchaseRequisition

Browser definition `purchaseRequisition`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBookDetail` |  | purchaseRequisition-accountingBookDetailCollection |  |  | [`purchaseRequisition-accountingBookDetailCollection`](#purchaserequisition-accountingbookdetailcollection) |  |
| `approvalStatus` |  | object |  |  |  |  |
| `approvalStatus.id` | Internal identifier | string |  |  |  | `11`, `1`, `2`, `3` |
| `approvalStatus.refName` | Reference Name | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `companyId` | Company Id | string |  |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `createdFrom` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `discountAmount` | Discount Amount | number | double |  |  |  |
| `discountDate` | Discount Date | string | date |  |  |  |
| `dueDate` | Due Date | string | date |  |  |  |
| `endDate` | End Date | string | date |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `estimatedTotal` | Estimated Total | number | double |  |  |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `expense` |  | purchaseRequisition-expenseCollection |  |  | [`purchaseRequisition-expenseCollection`](#purchaserequisition-expensecollection) |  |
| `externalId` | External ID | string |  |  |  |  |
| `fob` | FOB | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `item` |  | purchaseRequisition-itemCollection |  |  | [`purchaseRequisition-itemCollection`](#purchaserequisition-itemcollection) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `message` | Vendor Message | string |  |  |  |  |
| `nextApprover` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `originator` | Originator | string |  |  |  |  |
| `otherRefNum` | PO/Check Number | string |  |  |  |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `shipDate` | Ship Date | string | date |  |  |  |
| `source` |  | object |  |  |  |  |
| `source.id` | Internal identifier | string |  |  |  | `SuitePhone`, `smbXML`, `CSV`, `ADP`, `QIF`, `QB`, `PERQUEST`, `Yahoo`, `PaymentLink`, `customerCenter`, `webServices`, `eBay`, `restWebServices`, `NLWebStore`, `offlineClient`, `SCIS`, `Sync` |
| `source.refName` | Reference Name | string |  |  |  |  |
| `sourceSystem` |  | object |  |  |  |  |
| `sourceSystem.id` | Internal identifier | string |  |  |  | `SuitePhone`, `smbXML`, `CSV`, `ADP`, `QIF`, `QB`, `PERQUEST`, `Yahoo`, `PaymentLink`, `customerCenter`, `webServices`, `eBay`, `restWebServices`, `NLWebStore`, `offlineClient`, `SCIS`, `Sync` |
| `sourceSystem.refName` | Reference Name | string |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `A`, `B`, `R`, `C`, `D`, `E`, `F`, `G`, `H` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `storeOrder` |  | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `subtotal` | Subtotal | number | double |  |  |  |
| `terms` |  | term |  |  | [`term`](term.md#term) |  |
| `total` | Total | number | double |  |  |  |
| `trackingNumbers` | Tracking Numbers | string |  |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Transaction Number | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `webSite` |  | string |  |  |  |  |

## purchaseRequisition-accountingBookDetailCollection

Browser definition `purchaseRequisition-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | purchaseRequisition-accountingBookDetailElement[] |  |  | [`purchaseRequisition-accountingBookDetailElement`](#purchaserequisition-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseRequisition-accountingBookDetailElement

Browser definition `purchaseRequisition-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## purchaseRequisition-expenseCollection

Browser definition `purchaseRequisition-expenseCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | purchaseRequisition-expenseElement[] |  |  | [`purchaseRequisition-expenseElement`](#purchaserequisition-expenseelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseRequisition-expenseElement

Browser definition `purchaseRequisition-expenseElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `amount` | Amount | number | double |  |  |  |
| `category` |  | expenseCategory |  |  | [`expenseCategory`](expenseCategory.md#expensecategory) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `estimatedAmount` | Estimated Amount | number | double |  |  |  |
| `isBillable` | Billable | boolean |  |  |  |  |
| `isClosed` | Closed | boolean |  |  |  |  |
| `line` | Line | integer | int64 |  |  |  |
| `linkedOrder` |  | purchaseOrderCollection |  |  | [`purchaseOrderCollection`](purchaseOrder.md#purchaseordercollection) |  |
| `linkedOrderStatus` | Linked Order Status | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `poVendor` |  | vendor |  |  | [`vendor`](vendor.md#vendor) |  |
| `projecttask` |  | projectTask |  |  | [`projectTask`](projectTask.md#projecttask) |  |
| `refName` | Reference Name | string |  |  |  |  |

## purchaseRequisition-item-inventoryDetail

Browser definition `purchaseRequisition-item-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | purchaseRequisition-item-inventoryDetail-inventoryAssignmentCollection |  |  | [`purchaseRequisition-item-inventoryDetail-inventoryAssignmentCollection`](#purchaserequisition-item-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## purchaseRequisition-item-inventoryDetail-inventoryAssignmentCollection

Browser definition `purchaseRequisition-item-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | purchaseRequisition-item-inventoryDetail-inventoryAssignmentElement[] |  |  | [`purchaseRequisition-item-inventoryDetail-inventoryAssignmentElement`](#purchaserequisition-item-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseRequisition-item-inventoryDetail-inventoryAssignmentElement

Browser definition `purchaseRequisition-item-inventoryDetail-inventoryAssignmentElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `binNumber` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `inventoryDetail` | Inventory Detail | integer | int64 |  |  |  |
| `inventoryStatus` |  | inventoryStatus |  |  | [`inventoryStatus`](inventoryStatus.md#inventorystatus) |  |
| `issueInventoryNumber` |  | inventoryNumber |  |  | [`inventoryNumber`](inventoryNumber.md#inventorynumber) |  |
| `licensePlateNumber` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `packCarton` | Pack Carton | string |  |  |  |  |
| `pickCarton` | Pick Carton | string |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityAvailable` | Unpicked Bin Qty | number | float |  |  |  |
| `receiptInventoryNumber` | Serial/Lot Number | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `secondaryQuantity` | Secondary Quantity | number | float |  |  |  |
| `toBinNumber` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `toInventoryStatus` |  | inventoryStatus |  |  | [`inventoryStatus`](inventoryStatus.md#inventorystatus) |  |

## purchaseRequisition-itemCollection

Browser definition `purchaseRequisition-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | purchaseRequisition-itemElement[] |  |  | [`purchaseRequisition-itemElement`](#purchaserequisition-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseRequisition-itemElement

Browser definition `purchaseRequisition-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `billVarianceStatus` |  | object |  |  |  |  |
| `billVarianceStatus.id` | Internal identifier | string |  |  |  | `NOVARIANCES`, `JOURNALNOTPOSTED`, `JOURNALPOSTED` |
| `billVarianceStatus.refName` | Reference Name | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createPo` |  | object |  |  |  |  |
| `createPo.id` | Internal identifier | string |  |  |  | `CostRtrn`, `EndrTeg`, `SpecOrd`, `AuthDep`, `InTrnPay`, `POrdBlnk`, `ResvShip`, `Capture`, `GLAdj`, `OppClose`, `LandCost`, `CountAdj`, `OrdReval`, `Unbuild`, `IntcoAdj`, `CpFxVar`, `OrdAlloc`, `FxAsset`, `GACAdjst`, `WaveShip`, `RfqCtrct`, `POrdPrep`, `OwnRcpt`, `Transfrm`, `DepRfnd`, `BillVar`, `OrdBuild`, `FftRqFt`, `DepAppl`, `Payment`, `Refund`, `ColTeg`, `Reimb`, `OrdDgrss`, `KitShip`, `OrdAuth`, `WipBuild`, `CtrctOrd`, `OrdClose`, `RevRec`, `OrdRvCom`, `PickPack`, `TOrdCost`, `SysJrnl`, `Commissn`, `COGS`, `SrcContr`, `OsrcMfg`, `EstInvc`, `RfqVend`, `OrdDep`, `WOReval`, `CostRec`, `PurchOwn`, `OppEst`, `POrdReq`, `OrdBill`, `ExpRec`, `NetAsset`, `PrepAppl`, `OrdFftRq`, `BillRcpt`, `OrdArrng`, `PurchRet`, `CostDef`, `ShipRcpt`, `SaleRet`, `DiscTeg`, `RcptBill`, `CostDefR`, `DropShip`, `WaveOrd`, `PayTeg` |
| `createPo.refName` | Reference Name | string |  |  |  |  |
| `createdPo` |  | purchaseOrder |  |  | [`purchaseOrder`](purchaseOrder.md#purchaseorder) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `estimatedAmount` | Estimated Amount | number | double |  |  |  |
| `estimatedRate` | Estimated Rate | number | double |  |  |  |
| `expectedReceiptDate` | Expected Receipt Date | string | date |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `initOqpBucket` | Initial OQP Bucket | string |  |  |  |  |
| `inventoryDetail` |  | purchaseRequisition-item-inventoryDetail |  |  | [`purchaseRequisition-item-inventoryDetail`](#purchaserequisition-item-inventorydetail) |  |
| `isBillable` | Billable | boolean |  |  |  |  |
| `isClosed` | Closed | boolean |  |  |  |  |
| `isOpen` | Is Opened | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemSubtype` |  | object |  |  |  |  |
| `itemSubtype.id` | Internal identifier | string |  |  |  | `Sale`, `Purchase`, `Resale` |
| `itemSubtype.refName` | Reference Name | string |  |  |  |  |
| `itemType` |  | object |  |  |  |  |
| `itemType.id` | Internal identifier | string |  |  |  | `Group`, `Description`, `Discount`, `EndGroup`, `GiftCert`, `Subtotal`, `Service`, `ShipItem`, `TaxItem`, `InvtPart`, `Payment`, `Expense`, `NonInvtPart`, `TaxGroup`, `Kit`, `Markup`, `DwnLdItem`, `OthCharge`, `Assembly`, `SubscriPlan` |
| `itemType.refName` | Reference Name | string |  |  |  |  |
| `job` |  | job |  |  | [`job`](job.md#job) |  |
| `lastPurchasePrice` | Last Purchase Price | number | double |  |  |  |
| `licenseCode` | License Code | string |  |  |  |  |
| `line` | Transaction Line | integer | int64 |  |  |  |
| `linked` | Linked | boolean |  |  |  |  |
| `linkedOrder` |  | purchaseOrderCollection |  |  | [`purchaseOrderCollection`](purchaseOrder.md#purchaseordercollection) |  |
| `linkedOrderStatus` | Linked Order Status | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `marginal` | Marginal | boolean |  |  |  |  |
| `matrixType` | Matrix Type | string |  |  |  |  |
| `minQty` | Minimum Quantity | number | float |  |  |  |
| `options` | Options | string |  |  |  |  |
| `oqpBucket` | Oqp Bucket | string |  |  |  |  |
| `poCurrency` | Currency | string |  |  |  |  |
| `poRate` | PO Rate | number | double |  |  |  |
| `poVendor` |  | vendor |  |  | [`vendor`](vendor.md#vendor) |  |
| `printItems` | Print Items | boolean |  |  |  |  |
| `projecttask` |  | projectTask |  |  | [`projectTask`](projectTask.md#projecttask) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityAllocated` | Quantity Allocated | number | float |  |  |  |
| `quantityAvailable` | Available | number | float |  |  |  |
| `quantityCommitted` | Committed | number | float |  |  |  |
| `quantityDemandAllocated` | Allocated Demand | number | float |  |  |  |
| `quantityFulfilled` | Quantity Fulfilled | number | float |  |  |  |
| `quantityOnHand` | On Hand | number | float |  |  |  |
| `quantityPacked` | Quantity Packed | number | float |  |  |  |
| `quantityPicked` | Quantity Picked | number | float |  |  |  |
| `quantityReceived` | Quantity Received | number | float |  |  |  |
| `rate` | Rate | number | double |  |  |  |
| `rateIncludingTax` | Rate | number | double |  |  |  |
| `rateSchedule` | Rate Schedule | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `serialNumbers` | Serial/Lot Numbers | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `units` | Units | string |  |  |  |  |
| `vendorList` |  | string |  |  |  |  |
| `vendorName` | Vendor Name | string |  |  |  |  |

## purchaseRequisitionCollection

Browser definition `purchaseRequisitionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | purchaseRequisition[] |  |  | [`purchaseRequisition`](#purchaserequisition) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseRequisitionSelectOptions

Browser definition `purchaseRequisitionSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `approvalStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createdFrom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nextApprover` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `source` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceSystem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `terms` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

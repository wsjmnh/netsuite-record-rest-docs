# Schemas: workOrder

Property tables for definitions owned by `workOrder`.

Record page: [workOrder](../records/workOrder.md).

## Index

- [workOrder](#workorder) — 84 properties
- [workOrder-accountingBookDetailCollection](#workorder-accountingbookdetailcollection) — 6 properties
- [workOrder-accountingBookDetailElement](#workorder-accountingbookdetailelement) — 7 properties
- [workOrder-item-inventoryDetail](#workorder-item-inventorydetail) — 11 properties
- [workOrder-item-inventoryDetail-inventoryAssignmentCollection](#workorder-item-inventorydetail-inventoryassignmentcollection) — 6 properties
- [workOrder-item-inventoryDetail-inventoryAssignmentElement](#workorder-item-inventorydetail-inventoryassignmentelement) — 17 properties
- [workOrder-itemCollection](#workorder-itemcollection) — 6 properties
- [workOrder-itemElement](#workorder-itemelement) — 84 properties
- [workOrder-partnersCollection](#workorder-partnerscollection) — 6 properties
- [workOrder-partnersElement](#workorder-partnerselement) — 6 properties
- [workOrder-salesTeamCollection](#workorder-salesteamcollection) — 6 properties
- [workOrder-salesTeamElement](#workorder-salesteamelement) — 8 properties
- [workOrderCollection](#workordercollection) — 6 properties
- [workOrderSelectOptions](#workorderselectoptions) — 27 properties

## workOrder

Browser definition `workOrder`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBookDetail` |  | workOrder-accountingBookDetailCollection |  |  | [`workOrder-accountingBookDetailCollection`](#workorder-accountingbookdetailcollection) |  |
| `actualProductionEndDate` | Actual Production End Date | string | date |  |  |  |
| `actualProductionStartDate` | Actual Production Start Date | string | date |  |  |  |
| `assemblyItem` |  | assemblyItem |  |  | [`assemblyItem`](assemblyItem.md#assemblyitem) |  |
| `autoCalculateLag` | Auto-calculate Lag | boolean |  |  |  |  |
| `billOfMaterials` |  | bom |  |  | [`bom`](bom.md#bom) |  |
| `billOfMaterialsRevision` |  | bomRevision |  |  | [`bomRevision`](bomRevision.md#bomrevision) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `committed` | Buildable | number | float |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `createdFrom` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `discountAmount` | Discount Amount | number | double |  |  |  |
| `discountDate` | Discount Date | string | date |  |  |  |
| `dueDate` | Due Date | string | date |  |  |  |
| `effectiveBomControl` | Effective BoM Control | string |  |  |  |  |
| `endDate` | Production End Date | string | date |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `excludeCommission` | Exclude Commissions | boolean |  |  |  |  |
| `excludefromsupplyplanning` | Exclude from Supply Planning | boolean |  |  |  |  |
| `expandAssembly` | Mark Sub-assemblies Phantom | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `firmed` | Firmed | boolean |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isActualProdEndDateEnteredManually` | Enter Manually | boolean |  |  |  |  |
| `isActualProdStartDateEnteredManually` | Enter Manually | boolean |  |  |  |  |
| `isWip` | WIP | boolean |  |  |  |  |
| `item` |  | workOrder-itemCollection |  |  | [`workOrder-itemCollection`](#workorder-itemcollection) |  |
| `job` |  | job |  |  | [`job`](job.md#job) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `linkedPO` |  | purchaseOrder |  |  | [`purchaseOrder`](purchaseOrder.md#purchaseorder) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `manufacturingRouting` |  | manufacturingRouting |  |  | [`manufacturingRouting`](manufacturingRouting.md#manufacturingrouting) |  |
| `memo` | Memo | string |  |  |  |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `options` | Options | string |  |  |  |  |
| `orderStatus` |  | object |  |  |  |  |
| `orderStatus.id` | Internal identifier | string |  |  |  | `A`, `B`, `C`, `D`, `E`, `F`, `G`, `H`, `I`, `J`, `K`, `L`, `M`, `N`, `O`, `P`, `Q`, `R`, `S`, `T`, `U`, `V`, `W`, `X`, `Y`, `Z`, `0`, `1`, `2`, `3`, `4`, `5` |
| `orderStatus.refName` | Reference Name | string |  |  |  |  |
| `originator` | Originator | string |  |  |  |  |
| `otherRefNum` | PO/Check Number | string |  |  |  |  |
| `outsourced` | Outsourced | boolean |  |  |  |  |
| `outsourcingCharge` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `partners` |  | workOrder-partnersCollection |  |  | [`workOrder-partnersCollection`](#workorder-partnerscollection) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `prevPartner` | Previous Partner | integer | int64 |  |  |  |
| `prevRep` | Previous Representative | integer | int64 |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `requestedDate` | Supply Required By Date | string | date |  |  |  |
| `revision` |  | itemRevision |  |  | [`itemRevision`](itemRevision.md#itemrevision) |  |
| `revisionMemo` | Revision Memo | string |  |  |  |  |
| `salesEffectiveDate` | Sales Effective Date | string | date |  |  |  |
| `salesRep` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `salesTeam` |  | workOrder-salesTeamCollection |  |  | [`workOrder-salesTeamCollection`](#workorder-salesteamcollection) |  |
| `schedulingMethod` |  | object |  |  |  |  |
| `schedulingMethod.id` | Internal identifier | string |  |  |  | `BACKWARD`, `FORWARD` |
| `schedulingMethod.refName` | Reference Name | string |  |  |  |  |
| `source` |  | object |  |  |  |  |
| `source.id` | Internal identifier | string |  |  |  | `SuitePhone`, `smbXML`, `CSV`, `ADP`, `QIF`, `QB`, `PERQUEST`, `Yahoo`, `PaymentLink`, `customerCenter`, `webServices`, `eBay`, `restWebServices`, `NLWebStore`, `offlineClient`, `SCIS`, `Sync` |
| `source.refName` | Reference Name | string |  |  |  |  |
| `sourceSystem` |  | object |  |  |  |  |
| `sourceSystem.id` | Internal identifier | string |  |  |  | `SuitePhone`, `smbXML`, `CSV`, `ADP`, `QIF`, `QB`, `PERQUEST`, `Yahoo`, `PaymentLink`, `customerCenter`, `webServices`, `eBay`, `restWebServices`, `NLWebStore`, `offlineClient`, `SCIS`, `Sync` |
| `sourceSystem.refName` | Reference Name | string |  |  |  |  |
| `startDate` | Production Start Date | string | date |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `A`, `B`, `C`, `D`, `G`, `H` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `storeOrder` |  | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `terms` |  | term |  |  | [`term`](term.md#term) |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Order No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `unbuilt` | Unbuilt | number | float |  |  |  |
| `units` | Unit of Measure | string |  |  |  |  |
| `useComponentYield` | Use Component Yield | boolean |  |  |  |  |
| `vendor` |  | vendor |  |  | [`vendor`](vendor.md#vendor) |  |
| `webSite` |  | string |  |  |  |  |

## workOrder-accountingBookDetailCollection

Browser definition `workOrder-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | workOrder-accountingBookDetailElement[] |  |  | [`workOrder-accountingBookDetailElement`](#workorder-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrder-accountingBookDetailElement

Browser definition `workOrder-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## workOrder-item-inventoryDetail

Browser definition `workOrder-item-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | workOrder-item-inventoryDetail-inventoryAssignmentCollection |  |  | [`workOrder-item-inventoryDetail-inventoryAssignmentCollection`](#workorder-item-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## workOrder-item-inventoryDetail-inventoryAssignmentCollection

Browser definition `workOrder-item-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | workOrder-item-inventoryDetail-inventoryAssignmentElement[] |  |  | [`workOrder-item-inventoryDetail-inventoryAssignmentElement`](#workorder-item-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrder-item-inventoryDetail-inventoryAssignmentElement

Browser definition `workOrder-item-inventoryDetail-inventoryAssignmentElement`.

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

## workOrder-itemCollection

Browser definition `workOrder-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | workOrder-itemElement[] |  |  | [`workOrder-itemElement`](#workorder-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrder-itemElement

Browser definition `workOrder-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `allocationAlert` | Reallocate Order Item | string |  |  |  |  |
| `amount` | Amount | number | double |  |  |  |
| `assemblyLevel` | Hierarchy Level | integer | int64 |  |  |  |
| `billVarianceStatus` |  | object |  |  |  |  |
| `billVarianceStatus.id` | Internal identifier | string |  |  |  | `NOVARIANCES`, `JOURNALNOTPOSTED`, `JOURNALPOSTED` |
| `billVarianceStatus.refName` | Reference Name | string |  |  |  |  |
| `bomQuantity` | BoM Quantity | string |  |  |  |  |
| `bomRevisionComponent` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `commitInventory` |  | object |  |  |  |  |
| `commitInventory.id` | Internal identifier | string |  |  |  | `1`, `2`, `3` |
| `commitInventory.refName` | Reference Name | string |  |  |  |  |
| `commitmentFirm` | Commitment Confirmed | boolean |  |  |  |  |
| `componentYield` | Component Yield | number | double |  |  |  |
| `createPo` |  | object |  |  |  |  |
| `createPo.id` | Internal identifier | string |  |  |  | `CostRtrn`, `EndrTeg`, `SpecOrd`, `AuthDep`, `InTrnPay`, `POrdBlnk`, `ResvShip`, `Capture`, `GLAdj`, `OppClose`, `LandCost`, `CountAdj`, `OrdReval`, `Unbuild`, `IntcoAdj`, `CpFxVar`, `OrdAlloc`, `FxAsset`, `GACAdjst`, `WaveShip`, `RfqCtrct`, `POrdPrep`, `OwnRcpt`, `Transfrm`, `DepRfnd`, `BillVar`, `OrdBuild`, `FftRqFt`, `DepAppl`, `Payment`, `Refund`, `ColTeg`, `Reimb`, `OrdDgrss`, `KitShip`, `OrdAuth`, `WipBuild`, `CtrctOrd`, `OrdClose`, `RevRec`, `OrdRvCom`, `PickPack`, `TOrdCost`, `SysJrnl`, `Commissn`, `COGS`, `SrcContr`, `OsrcMfg`, `EstInvc`, `RfqVend`, `OrdDep`, `WOReval`, `CostRec`, `PurchOwn`, `OppEst`, `POrdReq`, `OrdBill`, `ExpRec`, `NetAsset`, `PrepAppl`, `OrdFftRq`, `BillRcpt`, `OrdArrng`, `PurchRet`, `CostDef`, `ShipRcpt`, `SaleRet`, `DiscTeg`, `RcptBill`, `CostDefR`, `DropShip`, `WaveOrd`, `PayTeg` |
| `createPo.refName` | Reference Name | string |  |  |  |  |
| `createWo` | Create WO | boolean |  |  |  |  |
| `createdPo` |  | purchaseOrder |  |  | [`purchaseOrder`](purchaseOrder.md#purchaseorder) |  |
| `daysLate` | Days Late | integer | int64 |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `expectedShipDate` | Expected Ship Date | string | date |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `initOqpBucket` | Initial OQP Bucket | string |  |  |  |  |
| `inventoryDetail` |  | workOrder-item-inventoryDetail |  |  | [`workOrder-item-inventoryDetail`](#workorder-item-inventorydetail) |  |
| `isAllocateFirmInvtOnly` | None | boolean |  |  |  |  |
| `isBomRevisionComponent` | BoM Revision Component | boolean |  |  |  |  |
| `isClosed` | Closed | boolean |  |  |  |  |
| `isFreezeFirmAllocation` | None | boolean |  |  |  |  |
| `isOpen` | Is Opened | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemSource` |  | object |  |  |  |  |
| `itemSource.id` | Internal identifier | string |  |  |  | `WORK_ORDER`, `PHANTOM`, `PURCHASE_ORDER`, `STOCK` |
| `itemSource.refName` | Reference Name | string |  |  |  |  |
| `itemSourceList` | Item Source options list | string |  |  |  |  |
| `itemSubtype` |  | object |  |  |  |  |
| `itemSubtype.id` | Internal identifier | string |  |  |  | `Sale`, `Purchase`, `Resale` |
| `itemSubtype.refName` | Reference Name | string |  |  |  |  |
| `itemType` |  | object |  |  |  |  |
| `itemType.id` | Internal identifier | string |  |  |  | `Group`, `Description`, `Discount`, `EndGroup`, `GiftCert`, `Subtotal`, `Service`, `ShipItem`, `TaxItem`, `InvtPart`, `Payment`, `Expense`, `NonInvtPart`, `TaxGroup`, `Kit`, `Markup`, `DwnLdItem`, `OthCharge`, `Assembly`, `SubscriPlan` |
| `itemType.refName` | Reference Name | string |  |  |  |  |
| `lastPurchasePrice` | Last Purchase Price | number | double |  |  |  |
| `licenseCode` | License Code | string |  |  |  |  |
| `line` | Transaction Line | integer | int64 |  |  |  |
| `linked` | Linked | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `marginal` | Marginal | boolean |  |  |  |  |
| `matrixType` | Matrix Type | string |  |  |  |  |
| `minQty` | Minimum Quantity | number | float |  |  |  |
| `operationDisplayText` |  | manufacturingOperationTask |  |  | [`manufacturingOperationTask`](manufacturingOperationTask.md#manufacturingoperationtask) |  |
| `options` | Options | string |  |  |  |  |
| `oqpBucket` | Oqp Bucket | string |  |  |  |  |
| `orderAllocationStrategy` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `orderDoc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `orderLine` | Order Line | integer | int64 |  |  |  |
| `orderPriority` | Order Priority | number | float |  |  |  |
| `plannedIssueDate` | Planned Component Issue Date | string | date-time |  |  |  |
| `poCurrency` | Currency | string |  |  |  |  |
| `poRate` | PO Rate | number | double |  |  |  |
| `poVendor` |  | vendor |  |  | [`vendor`](vendor.md#vendor) |  |
| `printItems` | Print Items | boolean |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityAllocated` | Quantity Allocated | number | float |  |  |  |
| `quantityAvailable` | Available | number | float |  |  |  |
| `quantityBackOrdered` | Back Ordered | number | float |  |  |  |
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
| `requestedDate` | Supply Required By Date | string | date |  |  |  |
| `roundUpAsComponent` | Round Up Quantity as Component | boolean |  |  |  |  |
| `serialNumbers` | Serial/Lot Numbers | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `units` | Units | string |  |  |  |  |
| `woId` | Work Order ID | string |  |  |  |  |

## workOrder-partnersCollection

Browser definition `workOrder-partnersCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | workOrder-partnersElement[] |  |  | [`workOrder-partnersElement`](#workorder-partnerselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrder-partnersElement

Browser definition `workOrder-partnersElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `contribution` | Contribution % | number | double |  |  |  |
| `isPrimary` | Primary | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `partner` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `partnerRole` |  | partnerCategory |  |  | [`partnerCategory`](partnerCategory.md#partnercategory) |  |
| `refName` | Reference Name | string |  |  |  |  |

## workOrder-salesTeamCollection

Browser definition `workOrder-salesTeamCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | workOrder-salesTeamElement[] |  |  | [`workOrder-salesTeamElement`](#workorder-salesteamelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrder-salesTeamElement

Browser definition `workOrder-salesTeamElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `contribution` | Contribution % | number | double |  |  |  |
| `employee` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `id` | ID | string |  |  |  |  |
| `isPrimary` | Primary | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `salesRole` |  | salesRole |  |  | [`salesRole`](salesRole.md#salesrole) |  |

## workOrderCollection

Browser definition `workOrderCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | workOrder[] |  |  | [`workOrder`](#workorder) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## workOrderSelectOptions

Browser definition `workOrderSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `assemblyItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billOfMaterials` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billOfMaterialsRevision` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createdFrom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `job` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `linkedPO` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `manufacturingRouting` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nexus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `orderStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `outsourcingCharge` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revision` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesRep` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `schedulingMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `source` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceSystem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `terms` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `units` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `vendor` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

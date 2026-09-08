# Schemas: itemReceipt

Property tables for definitions owned by `itemReceipt`.

Record page: [itemReceipt](../records/itemReceipt.md).

## Index

- [itemReceipt](#itemreceipt) — 41 properties
- [itemReceipt-accountingBookDetailCollection](#itemreceipt-accountingbookdetailcollection) — 6 properties
- [itemReceipt-accountingBookDetailElement](#itemreceipt-accountingbookdetailelement) — 7 properties
- [itemReceipt-appliedRulesCollection](#itemreceipt-appliedrulescollection) — 6 properties
- [itemReceipt-appliedRulesElement](#itemreceipt-appliedruleselement) — 9 properties
- [itemReceipt-expenseCollection](#itemreceipt-expensecollection) — 6 properties
- [itemReceipt-expenseElement](#itemreceipt-expenseelement) — 10 properties
- [itemReceipt-item-inventoryDetail](#itemreceipt-item-inventorydetail) — 11 properties
- [itemReceipt-item-inventoryDetail-inventoryAssignmentCollection](#itemreceipt-item-inventorydetail-inventoryassignmentcollection) — 6 properties
- [itemReceipt-item-inventoryDetail-inventoryAssignmentElement](#itemreceipt-item-inventorydetail-inventoryassignmentelement) — 17 properties
- [itemReceipt-item-landedCost](#itemreceipt-item-landedcost) — 7 properties
- [itemReceipt-item-landedCost-landedCostDataCollection](#itemreceipt-item-landedcost-landedcostdatacollection) — 6 properties
- [itemReceipt-item-landedCost-landedCostDataElement](#itemreceipt-item-landedcost-landedcostdataelement) — 4 properties
- [itemReceipt-itemCollection](#itemreceipt-itemcollection) — 6 properties
- [itemReceipt-itemElement](#itemreceipt-itemelement) — 53 properties
- [itemReceipt-landedCostsCollection](#itemreceipt-landedcostscollection) — 6 properties
- [itemReceipt-landedCostsElement](#itemreceipt-landedcostselement) — 8 properties
- [itemReceiptCollection](#itemreceiptcollection) — 6 properties
- [itemReceiptSelectOptions](#itemreceiptselectoptions) — 17 properties

## itemReceipt

Browser definition `itemReceipt`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBookDetail` |  | itemReceipt-accountingBookDetailCollection |  |  | [`itemReceipt-accountingBookDetailCollection`](#itemreceipt-accountingbookdetailcollection) |  |
| `appliedRules` |  | itemReceipt-appliedRulesCollection |  |  | [`itemReceipt-appliedRulesCollection`](#itemreceipt-appliedrulescollection) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `createdFrom` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `employee` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `expense` |  | itemReceipt-expenseCollection |  |  | [`itemReceipt-expenseCollection`](#itemreceipt-expensecollection) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inboundShipment` |  | inboundShipment |  |  | [`inboundShipment`](inboundShipment.md#inboundshipment) |  |
| `incoTerm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `item` |  | itemReceipt-itemCollection |  |  | [`itemReceipt-itemCollection`](#itemreceipt-itemcollection) |  |
| `itemFulfillment` |  | itemFulfillment |  |  | [`itemFulfillment`](itemFulfillment.md#itemfulfillment) |  |
| `landedCostMethod` |  | object |  |  |  |  |
| `landedCostMethod.id` | Internal identifier | string |  |  |  | `WEIGHT`, `QUANTITY`, `VALUE` |
| `landedCostMethod.refName` | Reference Name | string |  |  |  |  |
| `landedCostPerLine` | Landed Cost per Line | boolean |  |  |  |  |
| `landedCosts` |  | itemReceipt-landedCostsCollection |  |  | [`itemReceipt-landedCostsCollection`](#itemreceipt-landedcostscollection) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `orderId` | Order Id | integer | int64 |  |  |  |
| `orderType` | Order Type | string |  |  |  |  |
| `partner` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Ref No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |

## itemReceipt-accountingBookDetailCollection

Browser definition `itemReceipt-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemReceipt-accountingBookDetailElement[] |  |  | [`itemReceipt-accountingBookDetailElement`](#itemreceipt-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemReceipt-accountingBookDetailElement

Browser definition `itemReceipt-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## itemReceipt-appliedRulesCollection

Browser definition `itemReceipt-appliedRulesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemReceipt-appliedRulesElement[] |  |  | [`itemReceipt-appliedRulesElement`](#itemreceipt-appliedruleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemReceipt-appliedRulesElement

Browser definition `itemReceipt-appliedRulesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `creationDate` | Date | string | date |  |  |  |
| `details` | Details | string |  |  |  |  |
| `externalLogId` | External ID | integer | int64 |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `ruleType` | Rule Type: | string |  |  |  |  |
| `ruleTypeTranslation` | Rule Type | string |  |  |  |  |
| `transactionVersion` | Version | integer | int64 |  |  |  |

## itemReceipt-expenseCollection

Browser definition `itemReceipt-expenseCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemReceipt-expenseElement[] |  |  | [`itemReceipt-expenseElement`](#itemreceipt-expenseelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemReceipt-expenseElement

Browser definition `itemReceipt-expenseElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `amount` | Amount | number | double |  |  |  |
| `itemReceipt` |  | itemReceipt |  |  | [`itemReceipt`](#itemreceipt) |  |
| `line` | Line | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `markReceived` | Mark Received | boolean |  |  |  |  |
| `memo` | Description | string |  |  |  |  |
| `orderDoc` | Order Id | integer | int64 |  |  |  |
| `orderLine` | Order Line | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## itemReceipt-item-inventoryDetail

Browser definition `itemReceipt-item-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | itemReceipt-item-inventoryDetail-inventoryAssignmentCollection |  |  | [`itemReceipt-item-inventoryDetail-inventoryAssignmentCollection`](#itemreceipt-item-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## itemReceipt-item-inventoryDetail-inventoryAssignmentCollection

Browser definition `itemReceipt-item-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemReceipt-item-inventoryDetail-inventoryAssignmentElement[] |  |  | [`itemReceipt-item-inventoryDetail-inventoryAssignmentElement`](#itemreceipt-item-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemReceipt-item-inventoryDetail-inventoryAssignmentElement

Browser definition `itemReceipt-item-inventoryDetail-inventoryAssignmentElement`.

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

## itemReceipt-item-landedCost

Browser definition `itemReceipt-item-landedCost`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `id` | Internal ID | string |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `landedCostData` |  | itemReceipt-item-landedCost-landedCostDataCollection |  |  | [`itemReceipt-item-landedCost-landedCostDataCollection`](#itemreceipt-item-landedcost-landedcostdatacollection) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `total` | Total | number | double |  |  |  |
| `transactionId` |  | itemReceipt |  |  | [`itemReceipt`](#itemreceipt) |  |

## itemReceipt-item-landedCost-landedCostDataCollection

Browser definition `itemReceipt-item-landedCost-landedCostDataCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemReceipt-item-landedCost-landedCostDataElement[] |  |  | [`itemReceipt-item-landedCost-landedCostDataElement`](#itemreceipt-item-landedcost-landedcostdataelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemReceipt-item-landedCost-landedCostDataElement

Browser definition `itemReceipt-item-landedCost-landedCostDataElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `costCategory` |  | costCategory |  |  | [`costCategory`](costCategory.md#costcategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## itemReceipt-itemCollection

Browser definition `itemReceipt-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemReceipt-itemElement[] |  |  | [`itemReceipt-itemElement`](#itemreceipt-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemReceipt-itemElement

Browser definition `itemReceipt-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `billVarianceStatus` |  | object |  |  |  |  |
| `billVarianceStatus.id` | Internal identifier | string |  |  |  | `NOVARIANCES`, `JOURNALNOTPOSTED`, `JOURNALPOSTED` |
| `billVarianceStatus.refName` | Reference Name | string |  |  |  |  |
| `binNumbers` | Bin Numbers | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `consigned` | Consigned | boolean |  |  |  |  |
| `consignmentConsumed` | Consignment Consumed | string |  |  |  |  |
| `currency` | Currency | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `displayName` | Display Name | string |  |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `fromlocation` |  | string |  |  |  |  |
| `generateAccruals` | Generate Accruals | boolean |  |  |  |  |
| `inventoryDetail` |  | itemReceipt-item-inventoryDetail |  |  | [`itemReceipt-item-inventoryDetail`](#itemreceipt-item-inventorydetail) |  |
| `isCatchWeightItem` |  | boolean |  |  |  |  |
| `isConsignmentItem` |  | boolean |  |  |  |  |
| `isDropShipment` | Drop Shipment | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemFxAmount` | Foreign Amount | number | double |  |  |  |
| `itemName` | Item | string |  |  |  |  |
| `itemReceive` | Fulfill/Receive | boolean |  |  |  |  |
| `itemSubtype` | Subtype | string |  |  |  |  |
| `itemType` | Type | string |  |  |  |  |
| `itemUnitPrice` | Unit Price | number | double |  |  |  |
| `itemUpc` | UPC Code | string |  |  |  |  |
| `jobName` | Job | string |  |  |  |  |
| `kitMemberOf` | Member of Line | integer | int64 |  |  |  |
| `landedCost` |  | itemReceipt-item-landedCost |  |  | [`itemReceipt-item-landedCost`](#itemreceipt-item-landedcost) |  |
| `line` | Transaction Line | integer | int64 |  |  |  |
| `lineEntity` | Entity | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `onHand` | On Hand | number | float |  |  |  |
| `options` | Options | string |  |  |  |  |
| `orderDoc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `orderLine` | Order Line | integer | int64 |  |  |  |
| `primaryToSecondaryUnitConversionRate` |  | number | float |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityRemaining` | Quantity Remaining | number | float |  |  |  |
| `quantityRemainingDisplay` | Remaining | number | float |  |  |  |
| `rate` | Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `secondaryQuantity` | Secondary Quantity | number | float |  |  |  |
| `secondaryUnitConversionRate` |  | number | float |  |  |  |
| `secondaryUnits` | Secondary Units | string |  |  |  |  |
| `secondaryUnitsList` |  | string |  |  |  |  |
| `serialNumbers` | Serial/Lot Numbers | string |  |  |  |  |
| `unitCostOverride` | Override Rate | number | double |  |  |  |
| `units` | Units | string |  |  |  |  |
| `unitsDisplay` | Units | string |  |  |  |  |
| `vendorName` | Vendor Name | string |  |  |  |  |

## itemReceipt-landedCostsCollection

Browser definition `itemReceipt-landedCostsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemReceipt-landedCostsElement[] |  |  | [`itemReceipt-landedCostsElement`](#itemreceipt-landedcostselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemReceipt-landedCostsElement

Browser definition `itemReceipt-landedCostsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `category` |  | costCategory |  |  | [`costCategory`](costCategory.md#costcategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `source` |  | object |  |  |  |  |
| `source.id` | Internal identifier | string |  |  |  | `MANUAL`, `THISTRAN`, `OTHTRAN`, `OTHTREXC` |
| `source.refName` | Reference Name | string |  |  |  |  |
| `transaction` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## itemReceiptCollection

Browser definition `itemReceiptCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | itemReceipt[] |  |  | [`itemReceipt`](#itemreceipt) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemReceiptSelectOptions

Browser definition `itemReceiptSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createdFrom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `employee` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `inboundShipment` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `incoTerm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemFulfillment` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `landedCostMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `partner` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

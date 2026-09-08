# Schemas: intercompanyTransferOrder

Property tables for definitions owned by `intercompanyTransferOrder`.

Record page: [intercompanyTransferOrder](../records/intercompanyTransferOrder.md).

## Index

- [intercompanyTransferOrder](#intercompanytransferorder) — 81 properties
- [intercompanyTransferOrder-accountingBookDetailCollection](#intercompanytransferorder-accountingbookdetailcollection) — 6 properties
- [intercompanyTransferOrder-accountingBookDetailElement](#intercompanytransferorder-accountingbookdetailelement) — 7 properties
- [intercompanyTransferOrder-item-inventoryDetail](#intercompanytransferorder-item-inventorydetail) — 11 properties
- [intercompanyTransferOrder-item-inventoryDetail-inventoryAssignmentCollection](#intercompanytransferorder-item-inventorydetail-inventoryassignmentcollection) — 6 properties
- [intercompanyTransferOrder-item-inventoryDetail-inventoryAssignmentElement](#intercompanytransferorder-item-inventorydetail-inventoryassignmentelement) — 17 properties
- [intercompanyTransferOrder-itemCollection](#intercompanytransferorder-itemcollection) — 6 properties
- [intercompanyTransferOrder-itemElement](#intercompanytransferorder-itemelement) — 63 properties
- [intercompanyTransferOrder-shippingAddress](#intercompanytransferorder-shippingaddress) — 18 properties
- [intercompanyTransferOrderCollection](#intercompanytransferordercollection) — 6 properties
- [intercompanyTransferOrderSelectOptions](#intercompanytransferorderselectoptions) — 23 properties

## intercompanyTransferOrder

Browser definition `intercompanyTransferOrder`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBookDetail` |  | intercompanyTransferOrder-accountingBookDetailCollection |  |  | [`intercompanyTransferOrder-accountingBookDetailCollection`](#intercompanytransferorder-accountingbookdetailcollection) |  |
| `altHandlingCost` | Handling Cost | number | double |  |  |  |
| `altShippingCost` | Shipping Cost | number | double |  |  |  |
| `canBeUnapproved` | Can Be Unapproved | boolean |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
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
| `employee` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `endDate` | End Date | string | date |  |  |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `excludefromsupplyplanning` | Exclude from Supply Planning | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `firmed` | Firmed | boolean |  |  |  |  |
| `fob` | FOB | string |  |  |  |  |
| `handlingCost` | Handling Cost | number | double |  |  |  |
| `handlingTax1Rate` | Tax Rate | number | double |  |  |  |
| `handlingTax2Rate` | Tax Rate | number | double |  |  |  |
| `handlingTaxAmount` | Handling Tax Amount | number | double |  |  |  |
| `handlingTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `id` | Internal ID | string |  |  |  |  |
| `incoTerm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `item` |  | intercompanyTransferOrder-itemCollection |  |  | [`intercompanyTransferOrder-itemCollection`](#intercompanytransferorder-itemcollection) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `linkedTrackingNumbers` | Linked Tracking Numbers | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `orderStatus` |  | object |  |  |  |  |
| `orderStatus.id` | Internal identifier | string |  |  |  | `A`, `B` |
| `orderStatus.refName` | Reference Name | string |  |  |  |  |
| `orderType` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `originator` | Originator | string |  |  |  |  |
| `otherRefNum` | PO/Check Number | string |  |  |  |  |
| `overrideLeadTimeDays` | Override Lead Time (In Days) | integer | int64 |  |  |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `shipAddress` | Ship To | string |  |  |  |  |
| `shipAddressList` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `shipComplete` | Ship Complete | boolean |  |  |  |  |
| `shipDate` | Ship Date | string | date |  |  |  |
| `shipIsResidential` | Shipping address is residential | boolean |  |  |  |  |
| `shipMethod` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
| `shipOverride` | Override | boolean |  |  |  |  |
| `shippingAddress` |  | intercompanyTransferOrder-shippingAddress |  |  | [`intercompanyTransferOrder-shippingAddress`](#intercompanytransferorder-shippingaddress) |  |
| `shippingAddress_text` | Shipping Address | string |  |  |  |  |
| `shippingCost` | Shipping Cost | number | double |  |  |  |
| `shippingCostOverridden` | Shipping Cost Overridden | boolean |  |  |  |  |
| `shippingTax1Rate` | Tax Rate | number | double |  |  |  |
| `shippingTax2Rate` | Tax Rate | number | double |  |  |  |
| `shippingTaxAmount` | Shipping Tax Amount | number | double |  |  |  |
| `shippingTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `source` |  | object |  |  |  |  |
| `source.id` | Internal identifier | string |  |  |  | `SuitePhone`, `smbXML`, `CSV`, `ADP`, `QIF`, `QB`, `PERQUEST`, `Yahoo`, `PaymentLink`, `customerCenter`, `webServices`, `eBay`, `restWebServices`, `NLWebStore`, `offlineClient`, `SCIS`, `Sync` |
| `source.refName` | Reference Name | string |  |  |  |  |
| `sourceSystem` |  | object |  |  |  |  |
| `sourceSystem.id` | Internal identifier | string |  |  |  | `SuitePhone`, `smbXML`, `CSV`, `ADP`, `QIF`, `QB`, `PERQUEST`, `Yahoo`, `PaymentLink`, `customerCenter`, `webServices`, `eBay`, `restWebServices`, `NLWebStore`, `offlineClient`, `SCIS`, `Sync` |
| `sourceSystem.refName` | Reference Name | string |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `storeOrder` |  | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `subtotal` | Subtotal | number | double |  |  |  |
| `terms` |  | term |  |  | [`term`](term.md#term) |  |
| `toSubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `total` | Total | number | double |  |  |  |
| `trackingNumbers` | Tracking Numbers | string |  |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Transaction Number | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `transferLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `useItemCostAsTransferCost` | Use Item Cost As Transfer Cost | boolean |  |  |  |  |
| `webSite` |  | string |  |  |  |  |

## intercompanyTransferOrder-accountingBookDetailCollection

Browser definition `intercompanyTransferOrder-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | intercompanyTransferOrder-accountingBookDetailElement[] |  |  | [`intercompanyTransferOrder-accountingBookDetailElement`](#intercompanytransferorder-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## intercompanyTransferOrder-accountingBookDetailElement

Browser definition `intercompanyTransferOrder-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## intercompanyTransferOrder-item-inventoryDetail

Browser definition `intercompanyTransferOrder-item-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | intercompanyTransferOrder-item-inventoryDetail-inventoryAssignmentCollection |  |  | [`intercompanyTransferOrder-item-inventoryDetail-inventoryAssignmentCollection`](#intercompanytransferorder-item-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## intercompanyTransferOrder-item-inventoryDetail-inventoryAssignmentCollection

Browser definition `intercompanyTransferOrder-item-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | intercompanyTransferOrder-item-inventoryDetail-inventoryAssignmentElement[] |  |  | [`intercompanyTransferOrder-item-inventoryDetail-inventoryAssignmentElement`](#intercompanytransferorder-item-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## intercompanyTransferOrder-item-inventoryDetail-inventoryAssignmentElement

Browser definition `intercompanyTransferOrder-item-inventoryDetail-inventoryAssignmentElement`.

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

## intercompanyTransferOrder-itemCollection

Browser definition `intercompanyTransferOrder-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | intercompanyTransferOrder-itemElement[] |  |  | [`intercompanyTransferOrder-itemElement`](#intercompanytransferorder-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## intercompanyTransferOrder-itemElement

Browser definition `intercompanyTransferOrder-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `allocationAlert` | Reallocate Order Item | string |  |  |  |  |
| `amount` | Amount | number | double |  |  |  |
| `billVarianceStatus` |  | object |  |  |  |  |
| `billVarianceStatus.id` | Internal identifier | string |  |  |  | `NOVARIANCES`, `JOURNALNOTPOSTED`, `JOURNALPOSTED` |
| `billVarianceStatus.refName` | Reference Name | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `commitInventory` |  | object |  |  |  |  |
| `commitInventory.id` | Internal identifier | string |  |  |  | `1`, `2`, `3` |
| `commitInventory.refName` | Reference Name | string |  |  |  |  |
| `commitmentFirm` | Commitment Confirmed | boolean |  |  |  |  |
| `daysLate` | Days Late | integer | int64 |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `excludeFromPredictiveRisk` | Exclude From Predictive Risk | boolean |  |  |  |  |
| `expectedReceiptDate` | Expected Receipt Date | string | date |  |  |  |
| `expectedShipDate` | Expected Ship Date | string | date |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `initOqpBucket` | Initial OQP Bucket | string |  |  |  |  |
| `inventoryDetail` |  | intercompanyTransferOrder-item-inventoryDetail |  |  | [`intercompanyTransferOrder-item-inventoryDetail`](#intercompanytransferorder-item-inventorydetail) |  |
| `isAllocateFirmInvtOnly` | None | boolean |  |  |  |  |
| `isClosed` | Closed | boolean |  |  |  |  |
| `isFreezeFirmAllocation` | None | boolean |  |  |  |  |
| `isOpen` | Is Opened | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
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
| `options` | Options | string |  |  |  |  |
| `oqpBucket` | Oqp Bucket | string |  |  |  |  |
| `orderAllocationStrategy` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `orderPriority` | Order Priority | number | float |  |  |  |
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
| `requestedDate` | Requested Date | string | date |  |  |  |
| `serialNumbers` | Serial/Lot Numbers | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `units` | Units | string |  |  |  |  |

## intercompanyTransferOrder-shippingAddress

Browser definition `intercompanyTransferOrder-shippingAddress`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `addr1` | Address 1 | string |  |  |  |  |
| `addr2` | Address 2 | string |  |  |  |  |
| `addr3` | Address 3 | string |  |  |  |  |
| `addrPhone` | Phone | string |  |  |  |  |
| `addrText` | Address | string |  |  |  |  |
| `addressee` | Addressee | string |  |  |  |  |
| `attention` | Attention | string |  |  |  |  |
| `city` | City | string |  |  |  |  |
| `country` |  | object |  |  |  |  |
| `country.id` | Internal identifier | string |  |  |  | `PR`, `PS`, `PT`, `PW`, `PY`, `QA`, `AB`, `AD`, `AE`, `AF`, `AG`, `AI`, `AL`, `AM`, `AN`, `AO`, `AQ`, `AR`, `AS`, `AT`, `RE`, `AU`, `AW`, `AX`, `AZ`, `RO`, `BA`, `BB`, `RS`, `BD`, `BE`, `RU`, `BF`, `BG`, `RW`, `BH`, `BI`, `BJ`, `BL`, `BM`, `BN`, `BO`, `SA`, `BQ`, `SB`, `BR`, `SC`, `BS`, `SD`, `BT`, `SE`, `BV`, `SG`, `BW`, `SH`, `SI`, `BY`, `SJ`, `BZ`, `SK`, `SL`, `SM`, `SN`, `SO`, `CA`, `SR`, `CC`, `SS`, `CD`, `ST`, `CF`, `SV`, `CG`, `CH`, `SX`, `CI`, `SY`, `SZ`, `CK`, `CL`, `CM`, `CN`, `CO`, `CR`, `TC`, `CS`, `TD`, `CU`, `TF`, `CV`, `TG`, `CW`, `TH`, `CX`, `CY`, `TJ`, `CZ`, `TK`, `TL`, `TM`, `TN`, `TO`, `TR`, `TT`, `DE`, `TV`, `TW`, `DJ`, `TZ`, `DK`, `DM`, `DO`, `UA`, `UG`, `DZ`, `UM`, `EA`, `EC`, `US`, `EE`, `EG`, `EH`, `UY`, `UZ`, `VA`, `ER`, `VC`, `ES`, `ET`, `VE`, `VG`, `VI`, `VN`, `VU`, `FI`, `FJ`, `FK`, `FM`, `FO`, `FR`, `WF`, `GA`, `GB`, `WS`, `GD`, `GE`, `GF`, `GG`, `GH`, `GI`, `GL`, `GM`, `GN`, `GP`, `GQ`, `GR`, `GS`, `GT`, `GU`, `GW`, `GY`, `XK`, `HK`, `HM`, `HN`, `HR`, `HT`, `YE`, `HU`, `IC`, `ID`, `YT`, `IE`, `IL`, `IM`, `IN`, `IO`, `ZA`, `IQ`, `IR`, `IS`, `IT`, `ZM`, `JE`, `ZW`, `JM`, `JO`, `JP`, `KE`, `KG`, `KH`, `KI`, `KM`, `KN`, `KP`, `KR`, `KW`, `KY`, `KZ`, `LA`, `LB`, `LC`, `LI`, `LK`, `LR`, `LS`, `LT`, `LU`, `LV`, `LY`, `MA`, `MC`, `MD`, `ME`, `MF`, `MG`, `MH`, `MK`, `ML`, `MM`, `MN`, `MO`, `MP`, `MQ`, `MR`, `MS`, `MT`, `MU`, `MV`, `MW`, `MX`, `MY`, `MZ`, `NA`, `NC`, `NE`, `NF`, `NG`, `NI`, `NL`, `NO`, `NP`, `NR`, `NU`, `NZ`, `OM`, `PA`, `PE`, `PF`, `PG`, `PH`, `PK`, `PL`, `PM`, `PN` |
| `country.refName` | Reference Name | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `override` | Override | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `state` | State/Province | string |  |  |  |  |
| `zip` | Zip | string |  |  |  |  |

## intercompanyTransferOrderCollection

Browser definition `intercompanyTransferOrderCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | intercompanyTransferOrder[] |  |  | [`intercompanyTransferOrder`](#intercompanytransferorder) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## intercompanyTransferOrderSelectOptions

Browser definition `intercompanyTransferOrderSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createdFrom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `employee` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `handlingTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `incoTerm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nexus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `orderStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `orderType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipAddressList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shippingTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `source` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceSystem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `terms` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `toSubsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transferLocation` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

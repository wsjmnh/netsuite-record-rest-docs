# Schemas: purchaseOrder

Property tables for definitions owned by `purchaseOrder`.

Record page: [purchaseOrder](../records/purchaseOrder.md).

## Index

- [purchaseOrder](#purchaseorder) — 121 properties
- [purchaseOrder-accountingBookDetailCollection](#purchaseorder-accountingbookdetailcollection) — 6 properties
- [purchaseOrder-accountingBookDetailElement](#purchaseorder-accountingbookdetailelement) — 7 properties
- [purchaseOrder-appliedRulesCollection](#purchaseorder-appliedrulescollection) — 6 properties
- [purchaseOrder-appliedRulesElement](#purchaseorder-appliedruleselement) — 9 properties
- [purchaseOrder-billingAddress](#purchaseorder-billingaddress) — 18 properties
- [purchaseOrder-expenseCollection](#purchaseorder-expensecollection) — 6 properties
- [purchaseOrder-expenseElement](#purchaseorder-expenseelement) — 24 properties
- [purchaseOrder-item-inventoryDetail](#purchaseorder-item-inventorydetail) — 11 properties
- [purchaseOrder-item-inventoryDetail-inventoryAssignmentCollection](#purchaseorder-item-inventorydetail-inventoryassignmentcollection) — 6 properties
- [purchaseOrder-item-inventoryDetail-inventoryAssignmentElement](#purchaseorder-item-inventorydetail-inventoryassignmentelement) — 17 properties
- [purchaseOrder-itemCollection](#purchaseorder-itemcollection) — 6 properties
- [purchaseOrder-itemElement](#purchaseorder-itemelement) — 94 properties
- [purchaseOrder-shippingAddress](#purchaseorder-shippingaddress) — 18 properties
- [purchaseOrder-taxDetailsCollection](#purchaseorder-taxdetailscollection) — 6 properties
- [purchaseOrder-taxDetailsElement](#purchaseorder-taxdetailselement) — 14 properties
- [purchaseOrderCollection](#purchaseordercollection) — 6 properties
- [purchaseOrderSelectOptions](#purchaseorderselectoptions) — 31 properties

## purchaseOrder

Browser definition `purchaseOrder`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBookDetail` |  | purchaseOrder-accountingBookDetailCollection |  |  | [`purchaseOrder-accountingBookDetailCollection`](#purchaseorder-accountingbookdetailcollection) |  |
| `appliedRules` |  | purchaseOrder-appliedRulesCollection |  |  | [`purchaseOrder-appliedRulesCollection`](#purchaseorder-appliedrulescollection) |  |
| `approvalStatus` |  | object |  |  |  |  |
| `approvalStatus.id` | Internal identifier | string |  |  |  | `11`, `1`, `2`, `3` |
| `approvalStatus.refName` | Reference Name | string |  |  |  |  |
| `availableVendorCredit` | Available Vendor Credit | number | double |  |  |  |
| `balance` | Balance | number | double |  |  |  |
| `billAddr1` | Billing Address Line 1 | string |  |  |  |  |
| `billAddr2` | Billing Address Line 2 | string |  |  |  |  |
| `billAddr3` | Billing Address Line 3 | string |  |  |  |  |
| `billAddress` | Bill To | string |  |  |  |  |
| `billAddressList` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `billAddressee` | Billing Addressee | string |  |  |  |  |
| `billAttention` | Billing Attention | string |  |  |  |  |
| `billCity` | Billing Address City | string |  |  |  |  |
| `billCountry` |  | object |  |  |  |  |
| `billCountry.id` | Internal identifier | string |  |  |  | `PR`, `PS`, `PT`, `PW`, `PY`, `QA`, `AB`, `AD`, `AE`, `AF`, `AG`, `AI`, `AL`, `AM`, `AN`, `AO`, `AQ`, `AR`, `AS`, `AT`, `RE`, `AU`, `AW`, `AX`, `AZ`, `RO`, `BA`, `BB`, `RS`, `BD`, `BE`, `RU`, `BF`, `BG`, `RW`, `BH`, `BI`, `BJ`, `BL`, `BM`, `BN`, `BO`, `SA`, `BQ`, `SB`, `BR`, `SC`, `BS`, `SD`, `BT`, `SE`, `BV`, `SG`, `BW`, `SH`, `SI`, `BY`, `SJ`, `BZ`, `SK`, `SL`, `SM`, `SN`, `SO`, `CA`, `SR`, `CC`, `SS`, `CD`, `ST`, `CF`, `SV`, `CG`, `CH`, `SX`, `CI`, `SY`, `SZ`, `CK`, `CL`, `CM`, `CN`, `CO`, `CR`, `TC`, `CS`, `TD`, `CU`, `TF`, `CV`, `TG`, `CW`, `TH`, `CX`, `CY`, `TJ`, `CZ`, `TK`, `TL`, `TM`, `TN`, `TO`, `TR`, `TT`, `DE`, `TV`, `TW`, `DJ`, `TZ`, `DK`, `DM`, `DO`, `UA`, `UG`, `DZ`, `UM`, `EA`, `EC`, `US`, `EE`, `EG`, `EH`, `UY`, `UZ`, `VA`, `ER`, `VC`, `ES`, `ET`, `VE`, `VG`, `VI`, `VN`, `VU`, `FI`, `FJ`, `FK`, `FM`, `FO`, `FR`, `WF`, `GA`, `GB`, `WS`, `GD`, `GE`, `GF`, `GG`, `GH`, `GI`, `GL`, `GM`, `GN`, `GP`, `GQ`, `GR`, `GS`, `GT`, `GU`, `GW`, `GY`, `XK`, `HK`, `HM`, `HN`, `HR`, `HT`, `YE`, `HU`, `IC`, `ID`, `YT`, `IE`, `IL`, `IM`, `IN`, `IO`, `ZA`, `IQ`, `IR`, `IS`, `IT`, `ZM`, `JE`, `ZW`, `JM`, `JO`, `JP`, `KE`, `KG`, `KH`, `KI`, `KM`, `KN`, `KP`, `KR`, `KW`, `KY`, `KZ`, `LA`, `LB`, `LC`, `LI`, `LK`, `LR`, `LS`, `LT`, `LU`, `LV`, `LY`, `MA`, `MC`, `MD`, `ME`, `MF`, `MG`, `MH`, `MK`, `ML`, `MM`, `MN`, `MO`, `MP`, `MQ`, `MR`, `MS`, `MT`, `MU`, `MV`, `MW`, `MX`, `MY`, `MZ`, `NA`, `NC`, `NE`, `NF`, `NG`, `NI`, `NL`, `NO`, `NP`, `NR`, `NU`, `NZ`, `OM`, `PA`, `PE`, `PF`, `PG`, `PH`, `PK`, `PL`, `PM`, `PN` |
| `billCountry.refName` | Reference Name | string |  |  |  |  |
| `billOverride` | Override | string |  |  |  |  |
| `billPhone` | Billing Phone | string |  |  |  |  |
| `billState` | Billing Address State | string |  |  |  |  |
| `billZip` | Billing Address Zip Code | string |  |  |  |  |
| `billingAddress` |  | purchaseOrder-billingAddress |  |  | [`purchaseOrder-billingAddress`](#purchaseorder-billingaddress) |  |
| `billingAddress_text` | Billing Address | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `consigned` | Consigned | boolean |  |  |  |  |
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
| `email` | Email | string |  |  |  |  |
| `employee` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `endDate` | End Date | string | date |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `entityTaxRegNum` | Vendor Tax Reg. Number | string |  |  |  |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `excludefromsupplyplanning` | Exclude from Supply Planning | boolean |  |  |  |  |
| `expense` |  | purchaseOrder-expenseCollection |  |  | [`purchaseOrder-expenseCollection`](#purchaseorder-expensecollection) |  |
| `externalId` | External ID | string |  |  |  |  |
| `fax` | Fax | string |  |  |  |  |
| `firmed` | Firmed | boolean |  |  |  |  |
| `fob` | FOB | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `incoTerm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `intercoStatus` |  | object |  |  |  |  |
| `intercoStatus.id` | Internal identifier | string |  |  |  | `1`, `2`, `3` |
| `intercoStatus.refName` | Reference Name | string |  |  |  |  |
| `intercoTransaction` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `isCrossSubTransaction` | Cross-Subsidiary Transaction | boolean |  |  |  |  |
| `item` |  | purchaseOrder-itemCollection |  |  | [`purchaseOrder-itemCollection`](#purchaseorder-itemcollection) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `linkedTrackingNumbers` | Linked Tracking Numbers | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `message` | Vendor Message | string |  |  |  |  |
| `nextApprover` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `orderStatus` |  | object |  |  |  |  |
| `orderStatus.id` | Internal identifier | string |  |  |  | `P`, `A`, `B`, `C`, `D`, `E`, `F`, `G`, `H`, `Y` |
| `orderStatus.refName` | Reference Name | string |  |  |  |  |
| `originator` | Originator | string |  |  |  |  |
| `otherRefNum` | PO/Check Number | string |  |  |  |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `purchaseContract` |  | purchaseContract |  |  | [`purchaseContract`](purchaseContract.md#purchasecontract) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `shipAddress` | Ship To | string |  |  |  |  |
| `shipAddressList` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `shipDate` | Ship Date | string | date |  |  |  |
| `shipIsResidential` | Shipping address is residential | boolean |  |  |  |  |
| `shipMethod` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
| `shipOverride` | Override | boolean |  |  |  |  |
| `shipTo` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `shippingAddress` |  | purchaseOrder-shippingAddress |  |  | [`purchaseOrder-shippingAddress`](#purchaseorder-shippingaddress) |  |
| `shippingAddress_text` | Shipping Address | string |  |  |  |  |
| `source` |  | object |  |  |  |  |
| `source.id` | Internal identifier | string |  |  |  | `SuitePhone`, `smbXML`, `CSV`, `ADP`, `QIF`, `QB`, `PERQUEST`, `Yahoo`, `PaymentLink`, `customerCenter`, `webServices`, `eBay`, `restWebServices`, `NLWebStore`, `offlineClient`, `SCIS`, `Sync` |
| `source.refName` | Reference Name | string |  |  |  |  |
| `sourceSystem` |  | object |  |  |  |  |
| `sourceSystem.id` | Internal identifier | string |  |  |  | `SuitePhone`, `smbXML`, `CSV`, `ADP`, `QIF`, `QB`, `PERQUEST`, `Yahoo`, `PaymentLink`, `customerCenter`, `webServices`, `eBay`, `restWebServices`, `NLWebStore`, `offlineClient`, `SCIS`, `Sync` |
| `sourceSystem.refName` | Reference Name | string |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `P`, `A`, `B`, `C`, `D`, `E`, `F`, `G`, `H` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `storeOrder` |  | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `subsidiaryTaxRegNum` | Subsidiary Tax Reg. Number | string |  |  |  |  |
| `subtotal` | Subtotal | number | double |  |  |  |
| `supervisorApproval` | Supervisor Approval | boolean |  |  |  |  |
| `suppressUserEventsAndEmails` |  | string |  |  |  |  |
| `tax2Total` | PST | number | double |  |  |  |
| `taxDetails` |  | purchaseOrder-taxDetailsCollection |  |  | [`purchaseOrder-taxDetailsCollection`](#purchaseorder-taxdetailscollection) |  |
| `taxDetailsOverride` | Tax Details Override | boolean |  |  |  |  |
| `taxItem` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxPointDate` | Tax Point Date | string | date |  |  |  |
| `taxPointDateOverride` | Tax Point Date Override | boolean |  |  |  |  |
| `taxRate` | Tax Rate | number | float |  |  |  |
| `taxRegOverride` | Tax Registration Override | boolean |  |  |  |  |
| `taxTotal` | Tax Total | number | double |  |  |  |
| `terms` |  | term |  |  | [`term`](term.md#term) |  |
| `toBeEmailed` | To Be Emailed | boolean |  |  |  |  |
| `toBeFaxed` | To Be Faxed | boolean |  |  |  |  |
| `toBePrinted` | To Be Printed | boolean |  |  |  |  |
| `total` | Total | number | double |  |  |  |
| `totalAfterTaxes` | Total After Taxes | number | double |  |  |  |
| `trackingNumbers` | Tracking Numbers | string |  |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | PO # | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `unbilledOrders` | Unbilled Orders | number | double |  |  |  |
| `updateDropshipOrderQty` |  | string |  |  |  |  |
| `vatRegNum` | VAT Registration | string |  |  |  |  |
| `webSite` |  | string |  |  |  |  |

## purchaseOrder-accountingBookDetailCollection

Browser definition `purchaseOrder-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | purchaseOrder-accountingBookDetailElement[] |  |  | [`purchaseOrder-accountingBookDetailElement`](#purchaseorder-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseOrder-accountingBookDetailElement

Browser definition `purchaseOrder-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## purchaseOrder-appliedRulesCollection

Browser definition `purchaseOrder-appliedRulesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | purchaseOrder-appliedRulesElement[] |  |  | [`purchaseOrder-appliedRulesElement`](#purchaseorder-appliedruleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseOrder-appliedRulesElement

Browser definition `purchaseOrder-appliedRulesElement`.

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

## purchaseOrder-billingAddress

Browser definition `purchaseOrder-billingAddress`.

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

## purchaseOrder-expenseCollection

Browser definition `purchaseOrder-expenseCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | purchaseOrder-expenseElement[] |  |  | [`purchaseOrder-expenseElement`](#purchaseorder-expenseelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseOrder-expenseElement

Browser definition `purchaseOrder-expenseElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `amount` | Amount | number | double |  |  |  |
| `baseGrossAmt` | Gross Amount | number | double |  |  |  |
| `category` |  | expenseCategory |  |  | [`expenseCategory`](expenseCategory.md#expensecategory) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdFrom` |  | blanketPurchaseOrder |  |  | [`blanketPurchaseOrder`](blanketPurchaseOrder.md#blanketpurchaseorder) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `grossAmt` | Gross Amount | number | double |  |  |  |
| `isBillable` | Billable | boolean |  |  |  |  |
| `isClosed` | Closed | boolean |  |  |  |  |
| `line` | Line | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `projecttask` |  | projectTask |  |  | [`projectTask`](projectTask.md#projecttask) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `tax1Amt` | Tax Amount | number | double |  |  |  |
| `taxAmount` | Tax Amount | number | double |  |  |  |
| `taxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxDetailsReference` | Tax Details Reference | string |  |  |  |  |
| `taxRate1` | Tax Rate | number | double |  |  |  |
| `taxRate2` | PST | number | double |  |  |  |
| `uniqueKey` | Unique Key | integer | int64 |  |  |  |

## purchaseOrder-item-inventoryDetail

Browser definition `purchaseOrder-item-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | purchaseOrder-item-inventoryDetail-inventoryAssignmentCollection |  |  | [`purchaseOrder-item-inventoryDetail-inventoryAssignmentCollection`](#purchaseorder-item-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## purchaseOrder-item-inventoryDetail-inventoryAssignmentCollection

Browser definition `purchaseOrder-item-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | purchaseOrder-item-inventoryDetail-inventoryAssignmentElement[] |  |  | [`purchaseOrder-item-inventoryDetail-inventoryAssignmentElement`](#purchaseorder-item-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseOrder-item-inventoryDetail-inventoryAssignmentElement

Browser definition `purchaseOrder-item-inventoryDetail-inventoryAssignmentElement`.

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

## purchaseOrder-itemCollection

Browser definition `purchaseOrder-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | purchaseOrder-itemElement[] |  |  | [`purchaseOrder-itemElement`](#purchaseorder-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseOrder-itemElement

Browser definition `purchaseOrder-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `assembly` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `assemblyUnits` | Assembly Units | string |  |  |  |  |
| `baseGrossAmt` | Gross Amount | number | double |  |  |  |
| `billOfMaterials` |  | bom |  |  | [`bom`](bom.md#bom) |  |
| `billOfMaterialsRevision` |  | bomRevision |  |  | [`bomRevision`](bomRevision.md#bomrevision) |  |
| `billVarianceStatus` |  | object |  |  |  |  |
| `billVarianceStatus.id` | Internal identifier | string |  |  |  | `NOVARIANCES`, `JOURNALNOTPOSTED`, `JOURNALPOSTED` |
| `billVarianceStatus.refName` | Reference Name | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `consigned` | Consigned | boolean |  |  |  |  |
| `consignmentConsumed` | Consignment Consumed | string |  |  |  |  |
| `createOutsourcedWo` | Create WO | boolean |  |  |  |  |
| `createdFrom` |  | blanketPurchaseOrder |  |  | [`blanketPurchaseOrder`](blanketPurchaseOrder.md#blanketpurchaseorder) |  |
| `createdOutsourcedWoKey` | Create outsourced WO key | string |  |  |  |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `excludeFromPredictiveRisk` | Exclude From Predictive Risk | boolean |  |  |  |  |
| `expectedReceiptDate` | Expected Receipt Date | string | date |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `grossAmt` | Gross Amount | number | double |  |  |  |
| `initOqpBucket` | Initial OQP Bucket | string |  |  |  |  |
| `inventoryDetail` |  | purchaseOrder-item-inventoryDetail |  |  | [`purchaseOrder-item-inventoryDetail`](#purchaseorder-item-inventorydetail) |  |
| `isBillable` | Billable | boolean |  |  |  |  |
| `isCatchWeightItem` |  | boolean |  |  |  |  |
| `isClosed` | Closed | boolean |  |  |  |  |
| `isConsignmentItem` |  | boolean |  |  |  |  |
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
| `landedCostCategory` |  | costCategory |  |  | [`costCategory`](costCategory.md#costcategory) |  |
| `lastPurchasePrice` | Last Purchase Price | number | double |  |  |  |
| `leadTime` | Lead Time | integer | int64 |  |  |  |
| `licenseCode` | License Code | string |  |  |  |  |
| `line` | Transaction Line | integer | int64 |  |  |  |
| `linked` | Linked | boolean |  |  |  |  |
| `linkedOrder` |  | purchaseRequisitionCollection |  |  | [`purchaseRequisitionCollection`](purchaseRequisition.md#purchaserequisitioncollection) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `marginal` | Marginal | boolean |  |  |  |  |
| `matchBillToReceipt` | Match Bill To Receipt | boolean |  |  |  |  |
| `matrixType` | Matrix Type | string |  |  |  |  |
| `minQty` | Minimum Quantity | number | float |  |  |  |
| `options` | Options | string |  |  |  |  |
| `oqpBucket` | Oqp Bucket | string |  |  |  |  |
| `orderDoc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `orderLine` | Order Line | integer | int64 |  |  |  |
| `primaryToSecondaryUnitConversionRate` |  | number | float |  |  |  |
| `printItems` | Print Items | boolean |  |  |  |  |
| `productionEndDate` | Production End Date | string | date |  |  |  |
| `productionStartDate` | Production Start Date | string | date |  |  |  |
| `projecttask` |  | projectTask |  |  | [`projectTask`](projectTask.md#projecttask) |  |
| `purchaseContract` |  | purchaseContract |  |  | [`purchaseContract`](purchaseContract.md#purchasecontract) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityAllocated` | Quantity Allocated | number | float |  |  |  |
| `quantityAvailable` | Available | number | float |  |  |  |
| `quantityBilled` | Billed | number | float |  |  |  |
| `quantityCommitted` | Committed | number | float |  |  |  |
| `quantityDemandAllocated` | Allocated Demand | number | float |  |  |  |
| `quantityFulfilled` | Quantity Fulfilled | number | float |  |  |  |
| `quantityOnHand` | On Hand | number | float |  |  |  |
| `quantityOnShipments` | Quantity On Shipments | number | float |  |  |  |
| `quantityPacked` | Quantity Packed | number | float |  |  |  |
| `quantityPicked` | Quantity Picked | number | float |  |  |  |
| `quantityReceived` | Quantity Received | number | float |  |  |  |
| `rate` | Rate | number | double |  |  |  |
| `rateIncludingTax` | Rate | number | double |  |  |  |
| `rateSchedule` | Rate Schedule | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `secondaryQuantity` | Secondary Quantity | number | float |  |  |  |
| `secondaryUnitConversionRate` |  | number | float |  |  |  |
| `secondaryUnits` | Secondary Units | string |  |  |  |  |
| `secondaryUnitsList` |  | string |  |  |  |  |
| `serialNumbers` | Serial/Lot Numbers | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `targetLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `targetSubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tax1Amt` | Tax Amount | number | double |  |  |  |
| `taxAmount` | Tax Amount | number | double |  |  |  |
| `taxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxDetailsReference` | Tax Details Reference | string |  |  |  |  |
| `taxRate1` | Tax Rate | number | double |  |  |  |
| `taxRate2` | PST | number | double |  |  |  |
| `uniqueKey` | Unique Key | integer | int64 |  |  |  |
| `units` | Units | string |  |  |  |  |
| `vendorName` | Vendor Name | string |  |  |  |  |

## purchaseOrder-shippingAddress

Browser definition `purchaseOrder-shippingAddress`.

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

## purchaseOrder-taxDetailsCollection

Browser definition `purchaseOrder-taxDetailsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | purchaseOrder-taxDetailsElement[] |  |  | [`purchaseOrder-taxDetailsElement`](#purchaseorder-taxdetailselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseOrder-taxDetailsElement

Browser definition `purchaseOrder-taxDetailsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `calcDetail` | Details | string |  |  |  |  |
| `lineName` | Name | string |  |  |  |  |
| `lineType` | Line type | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `netAmount` | Net Amount | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `taxAmount` | Tax Amount | number | double |  |  |  |
| `taxBasis` | Tax Basis | number | double |  |  |  |
| `taxCode` |  | salesTaxItem |  |  | [`salesTaxItem`](salesTaxItem.md#salestaxitem) |  |
| `taxDetailsReference` |  | object |  |  |  |  |
| `taxDetailsReference.id` | Internal identifier | string |  |  |  |  |
| `taxDetailsReference.refName` | Reference Name | string |  |  |  |  |
| `taxRate` | Tax Rate | number | double |  |  |  |
| `taxType` | Tax Type | string |  |  |  |  |

## purchaseOrderCollection

Browser definition `purchaseOrderCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | purchaseOrder[] |  |  | [`purchaseOrder`](#purchaseorder) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## purchaseOrderSelectOptions

Browser definition `purchaseOrderSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `approvalStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billAddressList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billCountry` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createdFrom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `employee` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entityTaxRegNum` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `incoTerm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `intercoStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `intercoTransaction` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nextApprover` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nexus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `orderStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `purchaseContract` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipAddressList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipTo` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `source` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceSystem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiaryTaxRegNum` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `terms` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

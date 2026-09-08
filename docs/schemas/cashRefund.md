# Schemas: cashRefund

Property tables for definitions owned by `cashRefund`.

Record page: [cashRefund](../records/cashRefund.md).

## Index

- [cashRefund](#cashrefund) — 185 properties
- [cashRefund-accountingBookDetailCollection](#cashrefund-accountingbookdetailcollection) — 6 properties
- [cashRefund-accountingBookDetailElement](#cashrefund-accountingbookdetailelement) — 7 properties
- [cashRefund-appliedRulesCollection](#cashrefund-appliedrulescollection) — 6 properties
- [cashRefund-appliedRulesElement](#cashrefund-appliedruleselement) — 9 properties
- [cashRefund-billingAddress](#cashrefund-billingaddress) — 18 properties
- [cashRefund-item-inventoryDetail](#cashrefund-item-inventorydetail) — 11 properties
- [cashRefund-item-inventoryDetail-inventoryAssignmentCollection](#cashrefund-item-inventorydetail-inventoryassignmentcollection) — 6 properties
- [cashRefund-item-inventoryDetail-inventoryAssignmentElement](#cashrefund-item-inventorydetail-inventoryassignmentelement) — 17 properties
- [cashRefund-itemCollection](#cashrefund-itemcollection) — 6 properties
- [cashRefund-itemElement](#cashrefund-itemelement) — 97 properties
- [cashRefund-partnersCollection](#cashrefund-partnerscollection) — 6 properties
- [cashRefund-partnersElement](#cashrefund-partnerselement) — 6 properties
- [cashRefund-promotionsCollection](#cashrefund-promotionscollection) — 6 properties
- [cashRefund-promotionsElement](#cashrefund-promotionselement) — 4 properties
- [cashRefund-salesTeamCollection](#cashrefund-salesteamcollection) — 6 properties
- [cashRefund-salesTeamElement](#cashrefund-salesteamelement) — 8 properties
- [cashRefund-shippingAddress](#cashrefund-shippingaddress) — 18 properties
- [cashRefund-taxDetailsCollection](#cashrefund-taxdetailscollection) — 6 properties
- [cashRefund-taxDetailsElement](#cashrefund-taxdetailselement) — 14 properties
- [cashRefundCollection](#cashrefundcollection) — 6 properties
- [cashRefundSelectOptions](#cashrefundselectoptions) — 45 properties

## cashRefund

Browser definition `cashRefund`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `abbrevType` | Abbrev. Type | string |  |  |  |  |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `accountingBookDetail` |  | cashRefund-accountingBookDetailCollection |  |  | [`cashRefund-accountingBookDetailCollection`](#cashrefund-accountingbookdetailcollection) |  |
| `altHandlingCost` | Handling Cost | number | double |  |  |  |
| `altShippingCost` | Shipping Cost | number | double |  |  |  |
| `appliedRules` |  | cashRefund-appliedRulesCollection |  |  | [`cashRefund-appliedRulesCollection`](#cashrefund-appliedrulescollection) |  |
| `asOfDate` | As of Date | string | date |  |  |  |
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
| `billingAccount` |  | billingAccount |  |  | [`billingAccount`](billingAccount.md#billingaccount) |  |
| `billingAddress` |  | cashRefund-billingAddress |  |  | [`cashRefund-billingAddress`](#cashrefund-billingaddress) |  |
| `billingAddress_text` | Billing Address | string |  |  |  |  |
| `bulkProcSubmission` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `canHaveStackable` | Can Stack Promotions | boolean |  |  |  |  |
| `cardSwipe` | Card Swipe | string |  |  |  |  |
| `cardholderAuthentication` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `checkNumber` | Check # | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `cleared` | Cleared | boolean |  |  |  |  |
| `clearedDate` | Date Cleared | string | date |  |  |  |
| `contribPct` | Contribution Percentage | string |  |  |  |  |
| `couponCode` |  | couponCode |  |  | [`couponCode`](couponCode.md#couponcode) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `createdFrom` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `customerPaymentAuthorization` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `debitKsn` | Debit KSN | string |  |  |  |  |
| `debitPinBlock` | Debit Pin Block | string |  |  |  |  |
| `deferredRevenue` | Deferred Revenue | number | double |  |  |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `discountAmount` | Discount Amount | number | double |  |  |  |
| `discountDate` | Discount Date | string | date |  |  |  |
| `discountItem` |  | discountItem |  |  | [`discountItem`](discountItem.md#discountitem) |  |
| `discountRate` | Rate | number | double |  |  |  |
| `discountTotal` | Discount Total | number | double |  |  |  |
| `dueDate` | Due Date | string | date |  |  |  |
| `dynamicDescriptor` | Soft Descriptor | string |  |  |  |  |
| `email` | Email | string |  |  |  |  |
| `endDate` | End Date | string | date |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `entityTaxRegNum` | Customer Tax Reg. Number | string |  |  |  |  |
| `estGrossProfit` | Est. Gross Profit | number | double |  |  |  |
| `estGrossProfitPercent` | Est. Gross Profit Percent | number | double |  |  |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `excludeCommission` | Exclude Commissions | boolean |  |  |  |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fax` | Fax | string |  |  |  |  |
| `handlingCost` | Handling Cost | number | double |  |  |  |
| `handlingMode` |  | object |  |  |  |  |
| `handlingMode.id` | Internal identifier | string |  |  |  | `MIMIC`, `PROCESS`, `SAVE_ONLY` |
| `handlingMode.refName` | Reference Name | string |  |  |  |  |
| `handlingTax1Rate` | Tax Rate | number | double |  |  |  |
| `handlingTax2Rate` | Tax Rate | number | double |  |  |  |
| `handlingTaxAmount` | Handling Tax Amount | number | double |  |  |  |
| `handlingTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `id` | Internal ID | string |  |  |  |  |
| `inputReferenceCode` | Input P/N Ref. | string |  |  |  |  |
| `integrationId` | Integration ID | string |  |  |  |  |
| `isTaxable` | Taxable | boolean |  |  |  |  |
| `item` |  | cashRefund-itemCollection |  |  | [`cashRefund-itemCollection`](#cashrefund-itemcollection) |  |
| `job` |  | job |  |  | [`job`](job.md#job) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `leadSource` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `message` | Customer Message | string |  |  |  |  |
| `messageSel` |  | customerMessage |  |  | [`customerMessage`](customerMessage.md#customermessage) |  |
| `muccPromoCodeInstance` | Promo Code | string |  |  |  |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `number` | Document Number | integer | int64 |  |  |  |
| `originator` | Originator | string |  |  |  |  |
| `otherRefNum` | PO/Check Number | string |  |  |  |  |
| `outputAuthCode` | Auth. Code | string |  |  |  |  |
| `outputReferenceCode` | P/N Ref. | string |  |  |  |  |
| `partner` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `partners` |  | cashRefund-partnersCollection |  |  | [`cashRefund-partnersCollection`](#cashrefund-partnerscollection) |  |
| `payPalAuthId` | Authorization ID | string |  |  |  |  |
| `payPalTranId` | PayPal Tran. ID | string |  |  |  |  |
| `paymentCardCsc` | CSC | string |  |  |  |  |
| `paymentDeviceId` | Payment Device ID | string |  |  |  |  |
| `paymentInstrumentLimit` | Payment Instrument Limit | number | double |  |  |  |
| `paymentOperation` |  | object |  |  |  |  |
| `paymentOperation.id` | Internal identifier | string |  |  |  | `CREDIT`, `REFUND` |
| `paymentOperation.refName` | Reference Name | string |  |  |  |  |
| `paymentOption` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `paymentProcessingProfile` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `prevPartner` | Previous Partner | integer | int64 |  |  |  |
| `prevRep` | Previous Representative | integer | int64 |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `promoCode` |  | promotionCode |  |  | [`promotionCode`](promotionCode.md#promotioncode) |  |
| `promoCodePluginImpl` | Promo Code | string |  |  |  |  |
| `promotions` |  | cashRefund-promotionsCollection |  |  | [`cashRefund-promotionsCollection`](#cashrefund-promotionscollection) |  |
| `recognizedRevenue` | Recognized Revenue | number | double |  |  |  |
| `recurringBill` | Recurring Bill | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `refundCheck` | Create Check | boolean |  |  |  |  |
| `revCommitStatus` | Revenue Commitment Status | string |  |  |  |  |
| `revCommitStatusDescr` | Revenue Commitment Status | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `revenueStatus` | Revenue Status | string |  |  |  |  |
| `revenueStatusDescr` | Revenue Status | string |  |  |  |  |
| `salesEffectiveDate` | Sales Effective Date | string | date |  |  |  |
| `salesGroup` |  | entityGroup |  |  | [`entityGroup`](entityGroup.md#entitygroup) |  |
| `salesRep` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `salesReturn` | Sales Return | string |  |  |  |  |
| `salesTeam` |  | cashRefund-salesTeamCollection |  |  | [`cashRefund-salesTeamCollection`](#cashrefund-salesteamcollection) |  |
| `shipAddress` | Ship To | string |  |  |  |  |
| `shipAddressList` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `shipDate` | Ship Date | string | date |  |  |  |
| `shipIsResidential` | Shipping address is residential | boolean |  |  |  |  |
| `shipMethod` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
| `shipOverride` | Override | boolean |  |  |  |  |
| `shippingAddress` |  | cashRefund-shippingAddress |  |  | [`cashRefund-shippingAddress`](#cashrefund-shippingaddress) |  |
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
| `subsidiaryTaxRegNum` | Subsidiary Tax Reg. Number | string |  |  |  |  |
| `subtotal` | Subtotal | number | double |  |  |  |
| `syncPartnerTeams` | Update Customer | boolean |  |  |  |  |
| `syncSalesTeams` | Update Customer | boolean |  |  |  |  |
| `tax2Total` | PST | number | double |  |  |  |
| `taxDetails` |  | cashRefund-taxDetailsCollection |  |  | [`cashRefund-taxDetailsCollection`](#cashrefund-taxdetailscollection) |  |
| `taxDetailsOverride` | Tax Details Override | boolean |  |  |  |  |
| `taxItem` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxPointDate` | Tax Point Date | string | date |  |  |  |
| `taxPointDateOverride` | Tax Point Date Override | boolean |  |  |  |  |
| `taxRate` | Tax Rate | number | float |  |  |  |
| `taxRegOverride` | Tax Registration Override | boolean |  |  |  |  |
| `taxTotal` | Tax Total | number | double |  |  |  |
| `terms` |  | term |  |  | [`term`](term.md#term) |  |
| `thirdPartyAcct` | 3rd Party Account | string |  |  |  |  |
| `toBeEmailed` | To Be Emailed | boolean |  |  |  |  |
| `toBeFaxed` | To Be Faxed | boolean |  |  |  |  |
| `toBePrinted` | To Be Printed | boolean |  |  |  |  |
| `toPrint2` | Print {1} | boolean |  |  |  |  |
| `total` | Total | number | double |  |  |  |
| `totalAfterTaxes` | Total After Taxes | number | double |  |  |  |
| `totalCostEstimate` | Est. Cost | number | double |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Refund # | string |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `transactionToRefund` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `type` |  | object |  |  |  |  |
| `type.id` | Internal identifier | string |  |  |  | `VendPymt`, `CustCred`, `ItemShip`, `Check`, `CustChrg`, `Journal`, `Opprtnty`, `CustRfnd`, `TrnfrOrd`, `CashRfnd`, `Build`, `Unbuild`, `RevComm`, `SalesOrd`, `TegPybl`, `Deposit`, `WOIssue`, `FinChrg`, `PurchOrd`, `DepAppl`, `ExpRept`, `TegRcvbl`, `WOCompl`, `InvAdjst`, `Transfer`, `Paycheck`, `VendBill`, `YtdAdjst`, `ItemRcpt`, `PChkJrnl`, `Estimate`, `SysJrnl`, `Commissn`, `TaxPymt`, `RtnAuth`, `CustInvc`, `WorkOrd`, `FxReval`, `BinTrnfr`, `LiaAdjst`, `InvDistr`, `LiabPymt`, `RevComRv`, `VendAuth`, `CardRfnd`, `InvWksht`, `VendCred`, `BinWksht`, `Custom`, `CustDep`, `CustPymt`, `WOClose`, `CashSale`, `DeprCust`, `CardChrg`, `InvTrnfr` |
| `type.refName` | Reference Name | string |  |  |  |  |
| `vatRegNum` | VAT Registration | string |  |  |  |  |
| `vsoeAutoCalc` | Auto Calculate VSOE Allocation | boolean |  |  |  |  |
| `webSite` |  | string |  |  |  |  |
| `whichChargesToAdd` |  | object |  |  |  |  |
| `whichChargesToAdd.id` | Internal identifier | string |  |  |  | `ALL`, `TRANSACTION_DATE`, `AS_OF_DATE` |
| `whichChargesToAdd.refName` | Reference Name | string |  |  |  |  |

## cashRefund-accountingBookDetailCollection

Browser definition `cashRefund-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashRefund-accountingBookDetailElement[] |  |  | [`cashRefund-accountingBookDetailElement`](#cashrefund-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashRefund-accountingBookDetailElement

Browser definition `cashRefund-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## cashRefund-appliedRulesCollection

Browser definition `cashRefund-appliedRulesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashRefund-appliedRulesElement[] |  |  | [`cashRefund-appliedRulesElement`](#cashrefund-appliedruleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashRefund-appliedRulesElement

Browser definition `cashRefund-appliedRulesElement`.

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

## cashRefund-billingAddress

Browser definition `cashRefund-billingAddress`.

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

## cashRefund-item-inventoryDetail

Browser definition `cashRefund-item-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | cashRefund-item-inventoryDetail-inventoryAssignmentCollection |  |  | [`cashRefund-item-inventoryDetail-inventoryAssignmentCollection`](#cashrefund-item-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## cashRefund-item-inventoryDetail-inventoryAssignmentCollection

Browser definition `cashRefund-item-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashRefund-item-inventoryDetail-inventoryAssignmentElement[] |  |  | [`cashRefund-item-inventoryDetail-inventoryAssignmentElement`](#cashrefund-item-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashRefund-item-inventoryDetail-inventoryAssignmentElement

Browser definition `cashRefund-item-inventoryDetail-inventoryAssignmentElement`.

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

## cashRefund-itemCollection

Browser definition `cashRefund-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashRefund-itemElement[] |  |  | [`cashRefund-itemElement`](#cashrefund-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashRefund-itemElement

Browser definition `cashRefund-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `baseGrossAmt` | Gross Amount | number | double |  |  |  |
| `billVarianceStatus` |  | object |  |  |  |  |
| `billVarianceStatus.id` | Internal identifier | string |  |  |  | `NOVARIANCES`, `JOURNALNOTPOSTED`, `JOURNALPOSTED` |
| `billVarianceStatus.refName` | Reference Name | string |  |  |  |  |
| `binNumbers` | Bin Numbers | string |  |  |  |  |
| `catchUpPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `chargeType` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `costEstimate` | Est. Cost | number | double |  |  |  |
| `costEstimateRate` | Est. Rate | number | double |  |  |  |
| `costEstimateType` |  | object |  |  |  |  |
| `costEstimateType.id` | Internal identifier | string |  |  |  | `PREFVENDORRATE`, `AVGCOST`, `PURCHORDERRATE`, `LASTPURCHPRICE`, `MEMBERDEFINED`, `CUSTOM`, `ITEMDEFINED`, `PURCHPRICE` |
| `costEstimateType.refName` | Reference Name | string |  |  |  |  |
| `deferRevRec` | Deferred Revenue | boolean |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `doNotCreateRevenueElement` | Do Not Create Revenue Element | boolean |  |  |  |  |
| `estGrossProfit` | Est. Gross Profit | number | double |  |  |  |
| `estGrossProfitPercent` | Est. Gross Profit Percent | number | double |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `giftCertFrom` | From | string |  |  |  |  |
| `giftCertMessage` | Gift Message | string |  |  |  |  |
| `giftCertNumber` | Code | string |  |  |  |  |
| `giftCertRecipientEmail` | Recipient Email | string |  |  |  |  |
| `giftCertRecipientName` | Recipient Name | string |  |  |  |  |
| `grossAmt` | Gross Amount | number | double |  |  |  |
| `initOqpBucket` | Initial OQP Bucket | string |  |  |  |  |
| `inventoryDetail` |  | cashRefund-item-inventoryDetail |  |  | [`cashRefund-item-inventoryDetail`](#cashrefund-item-inventorydetail) |  |
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
| `lineUniqueKey` | Line Unique Key | string |  |  |  |  |
| `linked` | Linked | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `marginal` | Marginal | boolean |  |  |  |  |
| `matrixType` | Matrix Type | string |  |  |  |  |
| `minQty` | Minimum Quantity | number | float |  |  |  |
| `options` | Options | string |  |  |  |  |
| `oqpBucket` | Oqp Bucket | string |  |  |  |  |
| `orderDoc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `orderLine` | Order Line | integer | int64 |  |  |  |
| `price` |  | priceLevel |  |  | [`priceLevel`](priceLevel.md#pricelevel) |  |
| `printItems` | Print Items | boolean |  |  |  |  |
| `processedByRevCommit` | Processed by Rev Commit | boolean |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityAllocated` | Quantity Allocated | number | float |  |  |  |
| `quantityAvailable` | Available | number | float |  |  |  |
| `quantityCommitted` | Committed | number | float |  |  |  |
| `quantityDemandAllocated` | Allocated Demand | number | float |  |  |  |
| `quantityOnHand` | On Hand | number | float |  |  |  |
| `rate` | Rate | number | double |  |  |  |
| `rateIncludingTax` | Rate | number | double |  |  |  |
| `rateSchedule` | Rate Schedule | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecEndDate` | Rev. Rec. End Date | string | date |  |  |  |
| `revRecSchedule` |  | revRecSchedule |  |  | [`revRecSchedule`](revRecSchedule.md#revrecschedule) |  |
| `revRecStartDate` | Rev. Rec. Start Date | string | date |  |  |  |
| `revRecTermInMonths` | Rev. Rec. Term in Months | integer | int64 |  |  |  |
| `revrec_recurrencetype` | Rev Rec Recurrence Type | string |  |  |  |  |
| `serialNumbers` | Serial/Lot Numbers | string |  |  |  |  |
| `subscription` |  | subscription |  |  | [`subscription`](subscription.md#subscription) |  |
| `subscriptionLine` |  | subscriptionLine |  |  | [`subscriptionLine`](subscriptionLine.md#subscriptionline) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tax1Amt` | Tax Amount | number | double |  |  |  |
| `taxAmount` | Tax Amount | number | double |  |  |  |
| `taxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxDetailsReference` | Tax Details Reference | string |  |  |  |  |
| `taxRate1` | Tax Rate | number | double |  |  |  |
| `taxRate2` | PST | number | double |  |  |  |
| `uniqueKey` | Unique Key | integer | int64 |  |  |  |
| `units` | Units | string |  |  |  |  |
| `vsoeAllocation` | Allocation Amount | number | double |  |  |  |
| `vsoeAmount` | Calculated Amount | number | double |  |  |  |
| `vsoeDeferral` |  | object |  |  |  |  |
| `vsoeDeferral.id` | Internal identifier | string |  |  |  | `DEFERALLUNTIL`, `DEFERUNTIL` |
| `vsoeDeferral.refName` | Reference Name | string |  |  |  |  |
| `vsoeDelivered` | Delivered | boolean |  |  |  |  |
| `vsoeIsEstimate` | Estimate | boolean |  |  |  |  |
| `vsoePermitDiscount` |  | object |  |  |  |  |
| `vsoePermitDiscount.id` | Internal identifier | string |  |  |  | `IFDELIVERED`, `NEVER` |
| `vsoePermitDiscount.refName` | Reference Name | string |  |  |  |  |
| `vsoePrice` | Allocation Price | number | double |  |  |  |
| `vsoeSOPGroup` |  | object |  |  |  |  |
| `vsoeSOPGroup.id` | Internal identifier | string |  |  |  | `EXCLUDE`, `NORMAL`, `SOFTWARE` |
| `vsoeSOPGroup.refName` | Reference Name | string |  |  |  |  |

## cashRefund-partnersCollection

Browser definition `cashRefund-partnersCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashRefund-partnersElement[] |  |  | [`cashRefund-partnersElement`](#cashrefund-partnerselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashRefund-partnersElement

Browser definition `cashRefund-partnersElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `contribution` | Contribution % | number | double |  |  |  |
| `isPrimary` | Primary | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `partner` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `partnerRole` |  | partnerCategory |  |  | [`partnerCategory`](partnerCategory.md#partnercategory) |  |
| `refName` | Reference Name | string |  |  |  |  |

## cashRefund-promotionsCollection

Browser definition `cashRefund-promotionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashRefund-promotionsElement[] |  |  | [`cashRefund-promotionsElement`](#cashrefund-promotionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashRefund-promotionsElement

Browser definition `cashRefund-promotionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `couponCode` |  | couponCode |  |  | [`couponCode`](couponCode.md#couponcode) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `promoCode` |  | promotionCode |  |  | [`promotionCode`](promotionCode.md#promotioncode) |  |
| `refName` | Reference Name | string |  |  |  |  |

## cashRefund-salesTeamCollection

Browser definition `cashRefund-salesTeamCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashRefund-salesTeamElement[] |  |  | [`cashRefund-salesTeamElement`](#cashrefund-salesteamelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashRefund-salesTeamElement

Browser definition `cashRefund-salesTeamElement`.

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

## cashRefund-shippingAddress

Browser definition `cashRefund-shippingAddress`.

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

## cashRefund-taxDetailsCollection

Browser definition `cashRefund-taxDetailsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashRefund-taxDetailsElement[] |  |  | [`cashRefund-taxDetailsElement`](#cashrefund-taxdetailselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashRefund-taxDetailsElement

Browser definition `cashRefund-taxDetailsElement`.

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

## cashRefundCollection

Browser definition `cashRefundCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | cashRefund[] |  |  | [`cashRefund`](#cashrefund) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashRefundSelectOptions

Browser definition `cashRefundSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billAddressList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billCountry` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `bulkProcSubmission` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `cardholderAuthentication` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `couponCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createdFrom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customerPaymentAuthorization` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `discountItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entityTaxRegNum` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `handlingMode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `handlingTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `job` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `leadSource` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `messageSel` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nexus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `partner` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentOperation` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentOption` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentProcessingProfile` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `promoCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesRep` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipAddressList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shippingTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `source` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceSystem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiaryTaxRegNum` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `terms` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transactionToRefund` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `type` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `whichChargesToAdd` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

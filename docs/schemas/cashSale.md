# Schemas: cashSale

Property tables for definitions owned by `cashSale`.

Record page: [cashSale](../records/cashSale.md).

## Index

- [cashSale](#cashsale) — 238 properties
- [cashSale-accountingBookDetailCollection](#cashsale-accountingbookdetailcollection) — 6 properties
- [cashSale-accountingBookDetailElement](#cashsale-accountingbookdetailelement) — 7 properties
- [cashSale-appliedRulesCollection](#cashsale-appliedrulescollection) — 6 properties
- [cashSale-appliedRulesElement](#cashsale-appliedruleselement) — 9 properties
- [cashSale-billingAddress](#cashsale-billingaddress) — 18 properties
- [cashSale-expCostCollection](#cashsale-expcostcollection) — 6 properties
- [cashSale-expCostElement](#cashsale-expcostelement) — 36 properties
- [cashSale-giftCertRedemptionCollection](#cashsale-giftcertredemptioncollection) — 6 properties
- [cashSale-giftCertRedemptionElement](#cashsale-giftcertredemptionelement) — 4 properties
- [cashSale-item-inventoryDetail](#cashsale-item-inventorydetail) — 11 properties
- [cashSale-item-inventoryDetail-inventoryAssignmentCollection](#cashsale-item-inventorydetail-inventoryassignmentcollection) — 6 properties
- [cashSale-item-inventoryDetail-inventoryAssignmentElement](#cashsale-item-inventorydetail-inventoryassignmentelement) — 17 properties
- [cashSale-itemCollection](#cashsale-itemcollection) — 6 properties
- [cashSale-itemCost-inventoryDetail](#cashsale-itemcost-inventorydetail) — 11 properties
- [cashSale-itemCost-inventoryDetail-inventoryAssignmentCollection](#cashsale-itemcost-inventorydetail-inventoryassignmentcollection) — 6 properties
- [cashSale-itemCost-inventoryDetail-inventoryAssignmentElement](#cashsale-itemcost-inventorydetail-inventoryassignmentelement) — 17 properties
- [cashSale-itemCostCollection](#cashsale-itemcostcollection) — 6 properties
- [cashSale-itemCostElement](#cashsale-itemcostelement) — 42 properties
- [cashSale-itemElement](#cashsale-itemelement) — 114 properties
- [cashSale-partnersCollection](#cashsale-partnerscollection) — 6 properties
- [cashSale-partnersElement](#cashsale-partnerselement) — 6 properties
- [cashSale-promotionsCollection](#cashsale-promotionscollection) — 6 properties
- [cashSale-promotionsElement](#cashsale-promotionselement) — 4 properties
- [cashSale-salesTeamCollection](#cashsale-salesteamcollection) — 6 properties
- [cashSale-salesTeamElement](#cashsale-salesteamelement) — 8 properties
- [cashSale-shipGroupCollection](#cashsale-shipgroupcollection) — 6 properties
- [cashSale-shipGroupElement](#cashsale-shipgroupelement) — 29 properties
- [cashSale-shippingAddress](#cashsale-shippingaddress) — 18 properties
- [cashSale-taxDetailsCollection](#cashsale-taxdetailscollection) — 6 properties
- [cashSale-taxDetailsElement](#cashsale-taxdetailselement) — 14 properties
- [cashSale-timeCollection](#cashsale-timecollection) — 6 properties
- [cashSale-timeElement](#cashsale-timeelement) — 39 properties
- [cashSaleCollection](#cashsalecollection) — 6 properties
- [cashSaleSelectOptions](#cashsaleselectoptions) — 55 properties

## cashSale

Browser definition `cashSale`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `abbrevType` | Abbrev. Type | string |  |  |  |  |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `accountingBookDetail` |  | cashSale-accountingBookDetailCollection |  |  | [`cashSale-accountingBookDetailCollection`](#cashsale-accountingbookdetailcollection) |  |
| `altHandlingCost` | Handling Cost | number | double |  |  |  |
| `altShippingCost` | Shipping Cost | number | double |  |  |  |
| `appliedRules` |  | cashSale-appliedRulesCollection |  |  | [`cashSale-appliedRulesCollection`](#cashsale-appliedrulescollection) |  |
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
| `billingAddress` |  | cashSale-billingAddress |  |  | [`cashSale-billingAddress`](#cashsale-billingaddress) |  |
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
| `defaultILBAShipAddrVal` |  | string |  |  |  |  |
| `defaultILBAShippingAddressKey` |  | string |  |  |  |  |
| `defaultILShipMethKey` | Default Shipping Method Key | integer | int64 |  |  |  |
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
| `estimate` | Estimate | integer | int64 |  |  |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `excludeCommission` | Exclude Commissions | boolean |  |  |  |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `expCost` |  | cashSale-expCostCollection |  |  | [`cashSale-expCostCollection`](#cashsale-expcostcollection) |  |
| `expCostDiscAmount` | Amount | number | double |  |  |  |
| `expCostDiscPrint` | Print | boolean |  |  |  |  |
| `expCostDiscRate` | Rate | number | double |  |  |  |
| `expCostDiscTax1Amt` | Tax Amt | number | double |  |  |  |
| `expCostDiscTaxable` | Taxable | boolean |  |  |  |  |
| `expCostDiscount` |  | discountItem |  |  | [`discountItem`](discountItem.md#discountitem) |  |
| `expCostTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `expCostTaxRate1` | Tax Rate | number | double |  |  |  |
| `expCostTaxRate2` | PST | number | double |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fax` | Fax | string |  |  |  |  |
| `fob` | FOB | string |  |  |  |  |
| `giftCertApplied` | Gift Certificate | number | double |  |  |  |
| `giftCertRedemption` |  | cashSale-giftCertRedemptionCollection |  |  | [`cashSale-giftCertRedemptionCollection`](#cashsale-giftcertredemptioncollection) |  |
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
| `isMultiShipTo` | Enable Item Line Shipping | boolean |  |  |  |  |
| `isTaxable` | Taxable | boolean |  |  |  |  |
| `item` |  | cashSale-itemCollection |  |  | [`cashSale-itemCollection`](#cashsale-itemcollection) |  |
| `itemCost` |  | cashSale-itemCostCollection |  |  | [`cashSale-itemCostCollection`](#cashsale-itemcostcollection) |  |
| `itemCostDiscAmount` | Amount | number | double |  |  |  |
| `itemCostDiscPrint` | Print | boolean |  |  |  |  |
| `itemCostDiscRate` | Rate | number | double |  |  |  |
| `itemCostDiscTax1Amt` | Tax Amt | number | double |  |  |  |
| `itemCostDiscTaxable` | Taxable | boolean |  |  |  |  |
| `itemCostDiscount` |  | discountItem |  |  | [`discountItem`](discountItem.md#discountitem) |  |
| `itemCostTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `itemCostTaxRate1` | Tax Rate | number | double |  |  |  |
| `itemCostTaxRate2` | PST | number | double |  |  |  |
| `job` |  | job |  |  | [`job`](job.md#job) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `leadSource` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `linkedTrackingNumbers` | Linked Tracking Numbers | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `message` | Customer Message | string |  |  |  |  |
| `messageSel` |  | customerMessage |  |  | [`customerMessage`](customerMessage.md#customermessage) |  |
| `muccPromoCodeInstance` | Promo Code | string |  |  |  |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `number` | Document Number | integer | int64 |  |  |  |
| `oppcreatedfrom` |  | string |  |  |  |  |
| `oppcreatedfromtitle` |  | string |  |  |  |  |
| `opportunity` |  | opportunity |  |  | [`opportunity`](opportunity.md#opportunity) |  |
| `originator` | Originator | string |  |  |  |  |
| `otherRefNum` | PO/Check Number | string |  |  |  |  |
| `outputAuthCode` | Auth. Code | string |  |  |  |  |
| `outputReferenceCode` | P/N Ref. | string |  |  |  |  |
| `partner` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `partners` |  | cashSale-partnersCollection |  |  | [`cashSale-partnersCollection`](#cashsale-partnerscollection) |  |
| `payPalAuthId` | Authorization ID | string |  |  |  |  |
| `payPalTranId` | PayPal Tran. ID | string |  |  |  |  |
| `paymentCardCsc` | CSC | string |  |  |  |  |
| `paymentDeviceId` | Payment Device ID | string |  |  |  |  |
| `paymentInstrumentLimit` | Payment Instrument Limit | number | double |  |  |  |
| `paymentOperation` |  | object |  |  |  |  |
| `paymentOperation.id` | Internal identifier | string |  |  |  | `SALE`, `CAPTURE` |
| `paymentOperation.refName` | Reference Name | string |  |  |  |  |
| `paymentOption` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `paymentProcessingProfile` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `prevPartner` | Previous Partner | integer | int64 |  |  |  |
| `prevRep` | Previous Representative | integer | int64 |  |  |  |
| `previousOpportunity` | Previous Opportunity | string |  |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `promoCode` |  | promotionCode |  |  | [`promotionCode`](promotionCode.md#promotioncode) |  |
| `promoCodePluginImpl` | Promo Code | string |  |  |  |  |
| `promotions` |  | cashSale-promotionsCollection |  |  | [`cashSale-promotionsCollection`](#cashsale-promotionscollection) |  |
| `recognizedRevenue` | Recognized Revenue | number | double |  |  |  |
| `recurringBill` | Recurring Bill | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revCommitStatus` | Revenue Commitment Status | string |  |  |  |  |
| `revCommitStatusDescr` | Revenue Commitment Status | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `revenueStatus` | Revenue Status | string |  |  |  |  |
| `revenueStatusDescr` | Revenue Status | string |  |  |  |  |
| `saasCommitmentEndDate` | SaaS Metric Commitment End Date | string | date |  |  |  |
| `saasCommitmentStartDate` | SaaS Metric Commitment Start Date | string | date |  |  |  |
| `salesChannel` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `salesEffectiveDate` | Sales Effective Date | string | date |  |  |  |
| `salesGroup` |  | entityGroup |  |  | [`entityGroup`](entityGroup.md#entitygroup) |  |
| `salesRep` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `salesTeam` |  | cashSale-salesTeamCollection |  |  | [`cashSale-salesTeamCollection`](#cashsale-salesteamcollection) |  |
| `saleschannelorderpriority` |  | string |  |  |  |  |
| `sendOrderFulfillmentEmail` | Resend Order Fulfillment Email | boolean |  |  |  |  |
| `shipAddress` | Ship To | string |  |  |  |  |
| `shipAddressList` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `shipDate` | Ship Date | string | date |  |  |  |
| `shipGroup` |  | cashSale-shipGroupCollection |  |  | [`cashSale-shipGroupCollection`](#cashsale-shipgroupcollection) |  |
| `shipIsResidential` | Shipping address is residential | boolean |  |  |  |  |
| `shipMethod` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
| `shipOverride` | Override | boolean |  |  |  |  |
| `shippingAddress` |  | cashSale-shippingAddress |  |  | [`cashSale-shippingAddress`](#cashsale-shippingaddress) |  |
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
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `A`, `B`, `C` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `storeOrder` |  | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `subsidiaryTaxRegNum` | Subsidiary Tax Reg. Number | string |  |  |  |  |
| `subtotal` | Subtotal | number | double |  |  |  |
| `syncPartnerTeams` | Update Customer | boolean |  |  |  |  |
| `syncSalesTeams` | Update Customer | boolean |  |  |  |  |
| `tax2Total` | PST | number | double |  |  |  |
| `taxDetails` |  | cashSale-taxDetailsCollection |  |  | [`cashSale-taxDetailsCollection`](#cashsale-taxdetailscollection) |  |
| `taxDetailsOverride` | Tax Details Override | boolean |  |  |  |  |
| `taxItem` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxPointDate` | Tax Point Date | string | date |  |  |  |
| `taxPointDateOverride` | Tax Point Date Override | boolean |  |  |  |  |
| `taxRate` | Tax Rate | number | float |  |  |  |
| `taxRegOverride` | Tax Registration Override | boolean |  |  |  |  |
| `taxTotal` | Tax Total | number | double |  |  |  |
| `terms` |  | term |  |  | [`term`](term.md#term) |  |
| `thirdPartyAcct` | 3rd Party Account | string |  |  |  |  |
| `time` |  | cashSale-timeCollection |  |  | [`cashSale-timeCollection`](#cashsale-timecollection) |  |
| `timeDiscAmount` | Amount | number | double |  |  |  |
| `timeDiscPrint` | Print | boolean |  |  |  |  |
| `timeDiscRate` | Rate | number | double |  |  |  |
| `timeDiscTax1Amt` | Tax Amt | number | double |  |  |  |
| `timeDiscTaxable` | Taxable | boolean |  |  |  |  |
| `timeDiscount` |  | discountItem |  |  | [`discountItem`](discountItem.md#discountitem) |  |
| `timeTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `timeTaxRate1` | Tax Rate | number | double |  |  |  |
| `timeTaxRate2` | PST | number | double |  |  |  |
| `toBeEmailed` | To Be Emailed | boolean |  |  |  |  |
| `toBeFaxed` | To Be Faxed | boolean |  |  |  |  |
| `toBePrinted` | To Be Printed | boolean |  |  |  |  |
| `total` | Total | number | double |  |  |  |
| `totalAfterTaxes` | Total After Taxes | number | double |  |  |  |
| `totalCostEstimate` | Est. Cost | number | double |  |  |  |
| `trackingNumbers` | Tracking Numbers | string |  |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Sale # | string |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `transactionToRefund` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `type` |  | object |  |  |  |  |
| `type.id` | Internal identifier | string |  |  |  | `VendPymt`, `CustCred`, `ItemShip`, `Check`, `CustChrg`, `Journal`, `Opprtnty`, `CustRfnd`, `TrnfrOrd`, `CashRfnd`, `Build`, `Unbuild`, `RevComm`, `SalesOrd`, `TegPybl`, `Deposit`, `WOIssue`, `FinChrg`, `PurchOrd`, `DepAppl`, `ExpRept`, `TegRcvbl`, `WOCompl`, `InvAdjst`, `Transfer`, `Paycheck`, `VendBill`, `YtdAdjst`, `ItemRcpt`, `PChkJrnl`, `Estimate`, `SysJrnl`, `Commissn`, `TaxPymt`, `RtnAuth`, `CustInvc`, `WorkOrd`, `FxReval`, `BinTrnfr`, `LiaAdjst`, `InvDistr`, `LiabPymt`, `RevComRv`, `VendAuth`, `CardRfnd`, `InvWksht`, `VendCred`, `BinWksht`, `Custom`, `CustDep`, `CustPymt`, `WOClose`, `CashSale`, `DeprCust`, `CardChrg`, `InvTrnfr` |
| `type.refName` | Reference Name | string |  |  |  |  |
| `undepFunds` |  | object |  |  |  |  |
| `undepFunds.id` | Internal identifier | string |  |  |  |  |
| `undepFunds.refName` | Reference Name | string |  |  |  |  |
| `vatRegNum` | VAT Registration | string |  |  |  |  |
| `vsoeAutoCalc` | Auto Calculate VSOE Allocation | boolean |  |  |  |  |
| `webSite` |  | string |  |  |  |  |
| `whichChargesToAdd` |  | object |  |  |  |  |
| `whichChargesToAdd.id` | Internal identifier | string |  |  |  | `ALL`, `TRANSACTION_DATE`, `AS_OF_DATE` |
| `whichChargesToAdd.refName` | Reference Name | string |  |  |  |  |

## cashSale-accountingBookDetailCollection

Browser definition `cashSale-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashSale-accountingBookDetailElement[] |  |  | [`cashSale-accountingBookDetailElement`](#cashsale-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSale-accountingBookDetailElement

Browser definition `cashSale-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## cashSale-appliedRulesCollection

Browser definition `cashSale-appliedRulesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashSale-appliedRulesElement[] |  |  | [`cashSale-appliedRulesElement`](#cashsale-appliedruleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSale-appliedRulesElement

Browser definition `cashSale-appliedRulesElement`.

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

## cashSale-billingAddress

Browser definition `cashSale-billingAddress`.

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

## cashSale-expCostCollection

Browser definition `cashSale-expCostCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashSale-expCostElement[] |  |  | [`cashSale-expCostElement`](#cashsale-expcostelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSale-expCostElement

Browser definition `cashSale-expCostElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amortizationperiod` | Amortization Period | string |  |  |  |  |
| `amortizationtype` | Amortization Type | string |  |  |  |  |
| `amount` | Bill Amount | number | double |  |  |  |
| `apply` | Apply | boolean |  |  |  |  |
| `baseGrossAmt` | Gross Amount | number | double |  |  |  |
| `billedDate` | Date | string | date |  |  |  |
| `category` |  | expenseCategory |  |  | [`expenseCategory`](expenseCategory.md#expensecategory) |  |
| `categoryDisp` | Category | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `doc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `employee` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `employeeDisp` | Employee | string |  |  |  |  |
| `grossAmt` | Gross Amount | number | double |  |  |  |
| `job` |  | string |  |  |  |  |
| `jobDisp` | Project | string |  |  |  |  |
| `line` | Line | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `originalAmount` | Original Amount | number | double |  |  |  |
| `prevRevRecSched` |  | boolean |  |  |  |  |
| `prevRevRecTemp` |  | boolean |  |  |  |  |
| `processedByRevCommit` | Processed by Rev Commit | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecDefRevAcct` | Deferred Revenue Account | integer | int64 |  |  |  |
| `revRecEndDate` | Rev. Rec. End Date | string | date |  |  |  |
| `revRecSchedule` |  | revRecSchedule |  |  | [`revRecSchedule`](revRecSchedule.md#revrecschedule) |  |
| `revRecStartDate` | Rev. Rec. Start Date | string | date |  |  |  |
| `tax1Amt` | Tax Amount | number | double |  |  |  |
| `taxAmount` | Tax Amount | number | double |  |  |  |
| `taxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxDetailsReference` | Tax Details Reference | string |  |  |  |  |
| `taxRate1` | Tax Rate | number | double |  |  |  |
| `taxRate2` | PST | number | double |  |  |  |
| `url` | URL | string |  |  |  |  |

## cashSale-giftCertRedemptionCollection

Browser definition `cashSale-giftCertRedemptionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashSale-giftCertRedemptionElement[] |  |  | [`cashSale-giftCertRedemptionElement`](#cashsale-giftcertredemptionelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSale-giftCertRedemptionElement

Browser definition `cashSale-giftCertRedemptionElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `authCode` |  | giftCertificate |  |  | [`giftCertificate`](giftCertificate.md#giftcertificate) |  |
| `authCodeApplied` | Amount Applied | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## cashSale-item-inventoryDetail

Browser definition `cashSale-item-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | cashSale-item-inventoryDetail-inventoryAssignmentCollection |  |  | [`cashSale-item-inventoryDetail-inventoryAssignmentCollection`](#cashsale-item-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## cashSale-item-inventoryDetail-inventoryAssignmentCollection

Browser definition `cashSale-item-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashSale-item-inventoryDetail-inventoryAssignmentElement[] |  |  | [`cashSale-item-inventoryDetail-inventoryAssignmentElement`](#cashsale-item-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSale-item-inventoryDetail-inventoryAssignmentElement

Browser definition `cashSale-item-inventoryDetail-inventoryAssignmentElement`.

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

## cashSale-itemCollection

Browser definition `cashSale-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashSale-itemElement[] |  |  | [`cashSale-itemElement`](#cashsale-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSale-itemCost-inventoryDetail

Browser definition `cashSale-itemCost-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | cashSale-itemCost-inventoryDetail-inventoryAssignmentCollection |  |  | [`cashSale-itemCost-inventoryDetail-inventoryAssignmentCollection`](#cashsale-itemcost-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## cashSale-itemCost-inventoryDetail-inventoryAssignmentCollection

Browser definition `cashSale-itemCost-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashSale-itemCost-inventoryDetail-inventoryAssignmentElement[] |  |  | [`cashSale-itemCost-inventoryDetail-inventoryAssignmentElement`](#cashsale-itemcost-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSale-itemCost-inventoryDetail-inventoryAssignmentElement

Browser definition `cashSale-itemCost-inventoryDetail-inventoryAssignmentElement`.

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

## cashSale-itemCostCollection

Browser definition `cashSale-itemCostCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashSale-itemCostElement[] |  |  | [`cashSale-itemCostElement`](#cashsale-itemcostelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSale-itemCostElement

Browser definition `cashSale-itemCostElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amortizationperiod` | Amortization Period | string |  |  |  |  |
| `amortizationtype` | Amortization Type | string |  |  |  |  |
| `amount` | Total | number | double |  |  |  |
| `apply` | Apply | boolean |  |  |  |  |
| `baseGrossAmt` | Gross Amount | number | double |  |  |  |
| `billedDate` | Date | string | date |  |  |  |
| `binNumbers` | Bin Numbers | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `cost` | Rate | number | double |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `doc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `grossAmt` | Gross Amount | number | double |  |  |  |
| `inventoryDetail` |  | cashSale-itemCost-inventoryDetail |  |  | [`cashSale-itemCost-inventoryDetail`](#cashsale-itemcost-inventorydetail) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemCostCount` | Qty | string |  |  |  |  |
| `itemDisp` | Item Name | string |  |  |  |  |
| `job` |  | string |  |  |  |  |
| `jobDisp` | Project | string |  |  |  |  |
| `line` | Line | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Description | string |  |  |  |  |
| `options` | Options | string |  |  |  |  |
| `prevRevRecSched` |  | boolean |  |  |  |  |
| `prevRevRecTemp` |  | boolean |  |  |  |  |
| `processedByRevCommit` | Processed by Rev Commit | boolean |  |  |  |  |
| `rateSchedule` | Rate Schedule | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecDefRevAcct` | Deferred Revenue Account | integer | int64 |  |  |  |
| `revRecEndDate` | Rev. Rec. End Date | string | date |  |  |  |
| `revRecSchedule` |  | revRecSchedule |  |  | [`revRecSchedule`](revRecSchedule.md#revrecschedule) |  |
| `revRecStartDate` | Rev. Rec. Start Date | string | date |  |  |  |
| `serialNumbers` | Serial/Lot Numbers | string |  |  |  |  |
| `tax1Amt` | Tax Amount | number | double |  |  |  |
| `taxAmount` | Tax Amount | number | double |  |  |  |
| `taxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxDetailsReference` | Tax Details Reference | string |  |  |  |  |
| `taxRate1` | Tax Rate | number | double |  |  |  |
| `taxRate2` | PST | number | double |  |  |  |
| `unit` | Unit | string |  |  |  |  |
| `unitDisp` | Units | string |  |  |  |  |
| `url` | URL | string |  |  |  |  |

## cashSale-itemElement

Browser definition `cashSale-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `amountOrdered` | Amount Ordered | number | double |  |  |  |
| `baseGrossAmt` | Gross Amount | number | double |  |  |  |
| `binNumbers` | Bin Numbers | string |  |  |  |  |
| `catchUpPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `chargeType` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `costEstimate` | Est. Cost | number | double |  |  |  |
| `costEstimateRate` | Est. Rate | number | double |  |  |  |
| `costEstimateType` |  | object |  |  |  |  |
| `costEstimateType.id` | Internal identifier | string |  |  |  | `PREFVENDORRATE`, `AVGCOST`, `PURCHORDERRATE`, `LASTPURCHPRICE`, `MEMBERDEFINED`, `CUSTOM`, `ITEMDEFINED`, `PURCHPRICE` |
| `costEstimateType.refName` | Reference Name | string |  |  |  |  |
| `currentPercent` | Current % | number | double |  |  |  |
| `deferRevRec` | Deferred Revenue | boolean |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `doNotCreateRevenueElement` | Do Not Create Revenue Element | boolean |  |  |  |  |
| `estGrossProfit` | Est. Gross Profit | number | double |  |  |  |
| `estGrossProfitPercent` | Est. Gross Profit Percent | number | double |  |  |  |
| `excludeFromRateRequest` | Exclude Item from Rate Request | boolean |  |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `giftCertFrom` | From | string |  |  |  |  |
| `giftCertMessage` | Gift Message | string |  |  |  |  |
| `giftCertNumber` | Code | string |  |  |  |  |
| `giftCertRecipientEmail` | Recipient Email | string |  |  |  |  |
| `giftCertRecipientName` | Recipient Name | string |  |  |  |  |
| `grossAmt` | Gross Amount | number | double |  |  |  |
| `initOqpBucket` | Initial OQP Bucket | string |  |  |  |  |
| `inventoryDetail` |  | cashSale-item-inventoryDetail |  |  | [`cashSale-item-inventoryDetail`](#cashsale-item-inventorydetail) |  |
| `isClosed` | Closed | boolean |  |  |  |  |
| `isOpen` | Is Opened | boolean |  |  |  |  |
| `isTaxable` | Taxable | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemFulfillmentChoice` |  | object |  |  |  |  |
| `itemFulfillmentChoice.id` | Internal identifier | string |  |  |  | `1`, `2` |
| `itemFulfillmentChoice.refName` | Reference Name | string |  |  |  |  |
| `itemIsFulfilled` | Fulfilled | boolean |  |  |  |  |
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
| `quantityFulfilled` | Quantity Fulfilled | number | float |  |  |  |
| `quantityOnHand` | On Hand | number | float |  |  |  |
| `quantityOrdered` | Quantity Ordered | number | float |  |  |  |
| `quantityPacked` | Quantity Packed | number | float |  |  |  |
| `quantityPicked` | Quantity Picked | number | float |  |  |  |
| `quantityReceived` | Quantity Received | number | float |  |  |  |
| `quantityRemaining` | Quantity Remaining | number | float |  |  |  |
| `quantityRemainingDisplay` | Remaining | number | float |  |  |  |
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
| `shipAddress` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `shipCarrier` |  | object |  |  |  |  |
| `shipCarrier.id` | Internal identifier | string |  |  |  | `ups`, `nonups` |
| `shipCarrier.refName` | Reference Name | string |  |  |  |  |
| `shipGroup` | Ship Group | integer | int64 |  |  |  |
| `shipMethod` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
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

## cashSale-partnersCollection

Browser definition `cashSale-partnersCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashSale-partnersElement[] |  |  | [`cashSale-partnersElement`](#cashsale-partnerselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSale-partnersElement

Browser definition `cashSale-partnersElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `contribution` | Contribution % | number | double |  |  |  |
| `isPrimary` | Primary | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `partner` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `partnerRole` |  | partnerCategory |  |  | [`partnerCategory`](partnerCategory.md#partnercategory) |  |
| `refName` | Reference Name | string |  |  |  |  |

## cashSale-promotionsCollection

Browser definition `cashSale-promotionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashSale-promotionsElement[] |  |  | [`cashSale-promotionsElement`](#cashsale-promotionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSale-promotionsElement

Browser definition `cashSale-promotionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `couponCode` |  | couponCode |  |  | [`couponCode`](couponCode.md#couponcode) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `promoCode` |  | promotionCode |  |  | [`promotionCode`](promotionCode.md#promotioncode) |  |
| `refName` | Reference Name | string |  |  |  |  |

## cashSale-salesTeamCollection

Browser definition `cashSale-salesTeamCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashSale-salesTeamElement[] |  |  | [`cashSale-salesTeamElement`](#cashsale-salesteamelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSale-salesTeamElement

Browser definition `cashSale-salesTeamElement`.

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

## cashSale-shipGroupCollection

Browser definition `cashSale-shipGroupCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashSale-shipGroupElement[] |  |  | [`cashSale-shipGroupElement`](#cashsale-shipgroupelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSale-shipGroupElement

Browser definition `cashSale-shipGroupElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `destinationAddress` | Ship To | string |  |  |  |  |
| `handlingLineId` | Handling Line Id | integer | int64 |  |  |  |
| `handlingRate` | Handling Rate | number | double |  |  |  |
| `handlingTax2Amt` | Handling PST Amount | number | double |  |  |  |
| `handlingTax2Rate` | Handling PST Rate | number | double |  |  |  |
| `handlingTaxAmount` | Handling Tax Amount | number | double |  |  |  |
| `handlingTaxAmt` | Handling Tax Amount | number | double |  |  |  |
| `handlingTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `handlingTaxDetailsReference` | Handling Tax Details Reference | string |  |  |  |  |
| `handlingTaxRate` | Handling Tax Rate | number | double |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `isFulfilled` | Fulfilled | boolean |  |  |  |  |
| `isHandlingTaxable` | Handling Is Taxable | boolean |  |  |  |  |
| `isShippingTaxable` | Shipping Is Taxable | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `shippingMethod` | Ship Via | string |  |  |  |  |
| `shippingMethodId` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
| `shippingRate` | Shipping Rate | number | double |  |  |  |
| `shippingTax2Amt` | Shipping PST Amount | number | double |  |  |  |
| `shippingTax2Rate` | Shipping PST Rate | number | double |  |  |  |
| `shippingTaxAmount` | Shipping Tax Amount | number | double |  |  |  |
| `shippingTaxAmt` | Shipping Tax Amount | number | double |  |  |  |
| `shippingTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `shippingTaxDetailsReference` | Shipping Tax Details Reference | string |  |  |  |  |
| `shippingTaxRate` | Shipping Tax Rate | number | double |  |  |  |
| `sourceAddress` | Ship From | string |  |  |  |  |
| `uniqueKey` | Unique Key | string |  |  |  |  |
| `weight` | Weight | number | float |  |  |  |

## cashSale-shippingAddress

Browser definition `cashSale-shippingAddress`.

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

## cashSale-taxDetailsCollection

Browser definition `cashSale-taxDetailsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashSale-taxDetailsElement[] |  |  | [`cashSale-taxDetailsElement`](#cashsale-taxdetailselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSale-taxDetailsElement

Browser definition `cashSale-taxDetailsElement`.

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

## cashSale-timeCollection

Browser definition `cashSale-timeCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | cashSale-timeElement[] |  |  | [`cashSale-timeElement`](#cashsale-timeelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSale-timeElement

Browser definition `cashSale-timeElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amortizationperiod` | Amortization Period | string |  |  |  |  |
| `amortizationtype` | Amortization Type | string |  |  |  |  |
| `amount` | Amount | number | double |  |  |  |
| `apply` | Apply | boolean |  |  |  |  |
| `baseGrossAmt` | Gross Amount | number | double |  |  |  |
| `billedDate` | Date | string | date |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `doc` |  | timeBill |  |  | [`timeBill`](timeBill.md#timebill) |  |
| `employee` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `employeeDisp` | Employee | string |  |  |  |  |
| `grossAmt` | Gross Amount | number | double |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDisp` | Item | string |  |  |  |  |
| `job` |  | string |  |  |  |  |
| `jobDisp` | Project | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Description | string |  |  |  |  |
| `prevRevRecSched` |  | boolean |  |  |  |  |
| `prevRevRecTemp` |  | boolean |  |  |  |  |
| `processedByRevCommit` | Processed by Rev Commit | boolean |  |  |  |  |
| `quantity` | Hours | string |  |  |  |  |
| `rate` | Rate | number | double |  |  |  |
| `rateSchedule` | Rate Schedule | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecDefRevAcct` | Deferred Revenue Account | integer | int64 |  |  |  |
| `revRecEndDate` | Rev. Rec. End Date | string | date |  |  |  |
| `revRecSchedule` |  | revRecSchedule |  |  | [`revRecSchedule`](revRecSchedule.md#revrecschedule) |  |
| `revRecStartDate` | Rev. Rec. Start Date | string | date |  |  |  |
| `tax1Amt` | Tax Amount | number | double |  |  |  |
| `taxAmount` | Tax Amount | number | double |  |  |  |
| `taxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxDetailsReference` | Tax Details Reference | string |  |  |  |  |
| `taxRate1` | Tax Rate | number | double |  |  |  |
| `taxRate2` | PST | number | double |  |  |  |
| `unit` | Unit | string |  |  |  |  |
| `unitDisp` | Units | string |  |  |  |  |
| `url` | URL | string |  |  |  |  |

## cashSaleCollection

Browser definition `cashSaleCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | cashSale[] |  |  | [`cashSale`](#cashsale) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## cashSaleSelectOptions

Browser definition `cashSaleSelectOptions`.

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
| `expCostDiscount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `expCostTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `handlingMode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `handlingTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemCostDiscount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemCostTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `job` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `leadSource` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `messageSel` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nexus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `opportunity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `partner` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentOperation` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentOption` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentProcessingProfile` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `promoCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesChannel` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesRep` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipAddressList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shippingTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `source` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceSystem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiaryTaxRegNum` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `terms` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `timeDiscount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `timeTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transactionToRefund` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `type` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `undepFunds` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `whichChargesToAdd` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

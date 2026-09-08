# Schemas: salesOrder

Property tables for definitions owned by `salesOrder`.

Record page: [salesOrder](../records/salesOrder.md).

## Index

- [salesOrder](#salesorder) — 236 properties
- [salesOrder-accountingBookDetailCollection](#salesorder-accountingbookdetailcollection) — 6 properties
- [salesOrder-accountingBookDetailElement](#salesorder-accountingbookdetailelement) — 7 properties
- [salesOrder-appliedRulesCollection](#salesorder-appliedrulescollection) — 6 properties
- [salesOrder-appliedRulesElement](#salesorder-appliedruleselement) — 9 properties
- [salesOrder-billingAddress](#salesorder-billingaddress) — 18 properties
- [salesOrder-giftCertRedemptionCollection](#salesorder-giftcertredemptioncollection) — 6 properties
- [salesOrder-giftCertRedemptionElement](#salesorder-giftcertredemptionelement) — 4 properties
- [salesOrder-item-inventoryDetail](#salesorder-item-inventorydetail) — 12 properties
- [salesOrder-item-inventoryDetail-inventoryAssignmentCollection](#salesorder-item-inventorydetail-inventoryassignmentcollection) — 6 properties
- [salesOrder-item-inventoryDetail-inventoryAssignmentElement](#salesorder-item-inventorydetail-inventoryassignmentelement) — 17 properties
- [salesOrder-itemCollection](#salesorder-itemcollection) — 6 properties
- [salesOrder-itemElement](#salesorder-itemelement) — 159 properties
- [salesOrder-partnersCollection](#salesorder-partnerscollection) — 6 properties
- [salesOrder-partnersElement](#salesorder-partnerselement) — 6 properties
- [salesOrder-promotionsCollection](#salesorder-promotionscollection) — 6 properties
- [salesOrder-promotionsElement](#salesorder-promotionselement) — 4 properties
- [salesOrder-salesTeamCollection](#salesorder-salesteamcollection) — 6 properties
- [salesOrder-salesTeamElement](#salesorder-salesteamelement) — 8 properties
- [salesOrder-shipGroupCollection](#salesorder-shipgroupcollection) — 6 properties
- [salesOrder-shipGroupElement](#salesorder-shipgroupelement) — 29 properties
- [salesOrder-shippingAddress](#salesorder-shippingaddress) — 18 properties
- [salesOrder-taxDetailsCollection](#salesorder-taxdetailscollection) — 6 properties
- [salesOrder-taxDetailsElement](#salesorder-taxdetailselement) — 14 properties
- [salesOrderCollection](#salesordercollection) — 6 properties
- [salesOrderSelectOptions](#salesorderselectoptions) — 52 properties

## salesOrder

Browser definition `salesOrder`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBookDetail` |  | salesOrder-accountingBookDetailCollection |  |  | [`salesOrder-accountingBookDetailCollection`](#salesorder-accountingbookdetailcollection) |  |
| `actualShipDate` | Actual Shipping Date | string | date |  |  |  |
| `alaConfiguration` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `altHandlingCost` | Handling Cost | number | double |  |  |  |
| `altSalesTotal` | Alt. Sales Total | number | double |  |  |  |
| `altShippingCost` | Shipping Cost | number | double |  |  |  |
| `amountAuthorized` | Amount Authorized | number | double |  |  |  |
| `amountCovered` | Amount Covered | number | double |  |  |  |
| `amountDeposited` | Amount Deposited | number | double |  |  |  |
| `amountNotCovered` | Amount Not Covered | number | double |  |  |  |
| `amountPendingAuthorization` | Amount Pending Authorization | number | double |  |  |  |
| `amountPendingDeposit` | Amount Pending Deposit | number | double |  |  |  |
| `amountPotentiallyCovered` | Amount Potentially Covered | number | double |  |  |  |
| `amountRequiringCoverage` | Amount Requiring Coverage | number | double |  |  |  |
| `appliedRules` |  | salesOrder-appliedRulesCollection |  |  | [`salesOrder-appliedRulesCollection`](#salesorder-appliedrulescollection) |  |
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
| `billingAddress` |  | salesOrder-billingAddress |  |  | [`salesOrder-billingAddress`](#salesorder-billingaddress) |  |
| `billingAddress_text` | Billing Address | string |  |  |  |  |
| `billingSchedule` |  | billingSchedule |  |  | [`billingSchedule`](billingSchedule.md#billingschedule) |  |
| `canBeUnapproved` | Can Be Unapproved | boolean |  |  |  |  |
| `canHaveStackable` | Can Stack Promotions | boolean |  |  |  |  |
| `cardSwipe` | Card Swipe | string |  |  |  |  |
| `cardholderAuthentication` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `checkNumber` | Check # | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
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
| `drAccount` |  | account |  |  | [`account`](account.md#account) |  |
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
| `externalId` | External ID | string |  |  |  |  |
| `fax` | Fax | string |  |  |  |  |
| `fob` | FOB | string |  |  |  |  |
| `forInvoiceGrouping` | For Invoice Grouping | boolean |  |  |  |  |
| `fxAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `fxAltSalesTotal` | Foreign Alt. Sales Total | number | double |  |  |  |
| `fxNetAltSalesTotal` | Foreign Net Alt. Sales Total | number | double |  |  |  |
| `giftCertApplied` | Gift Certificate | number | double |  |  |  |
| `giftCertRedemption` |  | salesOrder-giftCertRedemptionCollection |  |  | [`salesOrder-giftCertRedemptionCollection`](#salesorder-giftcertredemptioncollection) |  |
| `groupedTo` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
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
| `intercoStatus` |  | object |  |  |  |  |
| `intercoStatus.id` | Internal identifier | string |  |  |  | `1`, `2`, `3` |
| `intercoStatus.refName` | Reference Name | string |  |  |  |  |
| `intercoTransaction` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `isCrossSubTransaction` | Allow Cross-Subsidiary Fulfillment | boolean |  |  |  |  |
| `isDefaultShippingRequest` | Is Default Shipping Request | boolean |  |  |  |  |
| `isMultiShipTo` | Enable Item Line Shipping | boolean |  |  |  |  |
| `isTaxable` | Taxable | boolean |  |  |  |  |
| `item` |  | salesOrder-itemCollection |  |  | [`salesOrder-itemCollection`](#salesorder-itemcollection) |  |
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
| `needsPick` | Needs Pick | boolean |  |  |  |  |
| `needsRevCommitment` |  | boolean |  |  |  |  |
| `netAltSalesTotal` | Net Alt. Sales Total | number | double |  |  |  |
| `nextBill` | Next Bill Date | string | date |  |  |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `oneTime` | One Time | number | double |  |  |  |
| `oppcreatedfrom` |  | string |  |  |  |  |
| `oppcreatedfromtitle` |  | string |  |  |  |  |
| `opportunity` |  | opportunity |  |  | [`opportunity`](opportunity.md#opportunity) |  |
| `ordRevCommitted` |  | boolean |  |  |  |  |
| `orderStatus` |  | object |  |  |  |  |
| `orderStatus.id` | Internal identifier | string |  |  |  | `A`, `B` |
| `orderStatus.refName` | Reference Name | string |  |  |  |  |
| `orderType` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `originator` | Originator | string |  |  |  |  |
| `otherRefNum` | PO/Check Number | string |  |  |  |  |
| `outputAuthCode` | Auth. Code | string |  |  |  |  |
| `outputReferenceCode` | P/N Ref. | string |  |  |  |  |
| `overrideShippingCost` | Override Shipping Cost | number | float |  |  |  |
| `partner` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `partners` |  | salesOrder-partnersCollection |  |  | [`salesOrder-partnersCollection`](#salesorder-partnerscollection) |  |
| `payPalAuthId` | Authorization ID | string |  |  |  |  |
| `payPalTranId` | PayPal Tran. ID | string |  |  |  |  |
| `paymentCardCsc` | CSC | string |  |  |  |  |
| `paymentDeviceId` | Payment Device ID | string |  |  |  |  |
| `paymentInstrumentLimit` | Payment Instrument Limit | number | double |  |  |  |
| `paymentOperation` |  | object |  |  |  |  |
| `paymentOperation.id` | Internal identifier | string |  |  |  | `SALE`, `VOID`, `AUTHORIZATION` |
| `paymentOperation.refName` | Reference Name | string |  |  |  |  |
| `paymentOption` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `paymentProcessingProfile` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `paymentsDue` | Payments Due | number | double |  |  |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `prevPartner` | Previous Partner | integer | int64 |  |  |  |
| `prevRep` | Previous Representative | integer | int64 |  |  |  |
| `previousOpportunity` | Previous Opportunity | string |  |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `promoCode` |  | promotionCode |  |  | [`promotionCode`](promotionCode.md#promotioncode) |  |
| `promoCodePluginImpl` | Promo Code | string |  |  |  |  |
| `promotions` |  | salesOrder-promotionsCollection |  |  | [`salesOrder-promotionsCollection`](#salesorder-promotionscollection) |  |
| `recognizedRevenue` | Recognized Revenue | number | double |  |  |  |
| `recurAnnually` | Annually | number | double |  |  |  |
| `recurMonthly` | Monthly | number | double |  |  |  |
| `recurQuarterly` | Quarterly | number | double |  |  |  |
| `recurWeekly` | Weekly | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `refreshFromSubscription` |  | string |  |  |  |  |
| `requiredDepositAmount` | Required Deposit Amount | number | double |  |  |  |
| `requiredDepositDue` | Required Deposit Due | number | double |  |  |  |
| `requiredDepositPercentage` | Required Deposit Percentage | number | double |  |  |  |
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
| `salesTeam` |  | salesOrder-salesTeamCollection |  |  | [`salesOrder-salesTeamCollection`](#salesorder-salesteamcollection) |  |
| `saleschannelorderpriority` |  | string |  |  |  |  |
| `shipAddress` | Ship To | string |  |  |  |  |
| `shipAddressList` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `shipComplete` | Ship Complete | boolean |  |  |  |  |
| `shipDate` | Ship Date | string | date |  |  |  |
| `shipGroup` |  | salesOrder-shipGroupCollection |  |  | [`salesOrder-shipGroupCollection`](#salesorder-shipgroupcollection) |  |
| `shipIsResidential` | Shipping address is residential | boolean |  |  |  |  |
| `shipMethod` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
| `shipOverride` | Override | boolean |  |  |  |  |
| `shippingAddress` |  | salesOrder-shippingAddress |  |  | [`salesOrder-shippingAddress`](#salesorder-shippingaddress) |  |
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
| `sourceWebSite` |  | webSite |  |  | [`webSite`](webSite.md#website) |  |
| `startDate` | Start Date | string | date |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `A`, `B`, `C`, `D`, `E`, `F`, `G`, `H` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `storeOrder` |  | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `subsidiaryTaxRegNum` | Subsidiary Tax Reg. Number | string |  |  |  |  |
| `subtotal` | Subtotal | number | double |  |  |  |
| `suppressUserEventsAndEmails` |  | string |  |  |  |  |
| `syncPartnerTeams` | Update Customer | boolean |  |  |  |  |
| `syncSalesTeams` | Update Customer | boolean |  |  |  |  |
| `tax2Total` | PST | number | double |  |  |  |
| `taxDetails` |  | salesOrder-taxDetailsCollection |  |  | [`salesOrder-taxDetailsCollection`](#salesorder-taxdetailscollection) |  |
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
| `total` | Total | number | double |  |  |  |
| `totalAfterTaxes` | Total After Taxes | number | double |  |  |  |
| `totalCostEstimate` | Est. Cost | number | double |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Order # | string |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `transactionToRefund` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `updateDropshipOrderQty` |  | string |  |  |  |  |
| `vatRegNum` | VAT Registration | string |  |  |  |  |
| `vsoeAutoCalc` | Auto Calculate VSOE Allocation | boolean |  |  |  |  |
| `webSite` |  | string |  |  |  |  |
| `webStore` | Web Store | string |  |  |  |  |

## salesOrder-accountingBookDetailCollection

Browser definition `salesOrder-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesOrder-accountingBookDetailElement[] |  |  | [`salesOrder-accountingBookDetailElement`](#salesorder-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesOrder-accountingBookDetailElement

Browser definition `salesOrder-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## salesOrder-appliedRulesCollection

Browser definition `salesOrder-appliedRulesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesOrder-appliedRulesElement[] |  |  | [`salesOrder-appliedRulesElement`](#salesorder-appliedruleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesOrder-appliedRulesElement

Browser definition `salesOrder-appliedRulesElement`.

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

## salesOrder-billingAddress

Browser definition `salesOrder-billingAddress`.

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

## salesOrder-giftCertRedemptionCollection

Browser definition `salesOrder-giftCertRedemptionCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesOrder-giftCertRedemptionElement[] |  |  | [`salesOrder-giftCertRedemptionElement`](#salesorder-giftcertredemptionelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesOrder-giftCertRedemptionElement

Browser definition `salesOrder-giftCertRedemptionElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `authCode` |  | giftCertificate |  |  | [`giftCertificate`](giftCertificate.md#giftcertificate) |  |
| `authCodeApplied` | Amount Applied | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## salesOrder-item-inventoryDetail

Browser definition `salesOrder-item-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inventoryAssignment` |  | salesOrder-item-inventoryDetail-inventoryAssignmentCollection |  |  | [`salesOrder-item-inventoryDetail-inventoryAssignmentCollection`](#salesorder-item-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## salesOrder-item-inventoryDetail-inventoryAssignmentCollection

Browser definition `salesOrder-item-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesOrder-item-inventoryDetail-inventoryAssignmentElement[] |  |  | [`salesOrder-item-inventoryDetail-inventoryAssignmentElement`](#salesorder-item-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesOrder-item-inventoryDetail-inventoryAssignmentElement

Browser definition `salesOrder-item-inventoryDetail-inventoryAssignmentElement`.

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

## salesOrder-itemCollection

Browser definition `salesOrder-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesOrder-itemElement[] |  |  | [`salesOrder-itemElement`](#salesorder-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesOrder-itemElement

Browser definition `salesOrder-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `allocationAlert` | Reallocate Order Item | string |  |  |  |  |
| `altSalesAmt` | Alt. Sales Amount | number | double |  |  |  |
| `amount` | Amount | number | double |  |  |  |
| `baseAmount` | Base Amount | number | double |  |  |  |
| `baseGrossAmt` | Gross Amount | number | double |  |  |  |
| `baseNetAmount` | Amount (Net) | number | double |  |  |  |
| `billingSchedule` |  | billingSchedule |  |  | [`billingSchedule`](billingSchedule.md#billingschedule) |  |
| `binNumbers` | Bin Numbers | string |  |  |  |  |
| `catchUpPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `chargeRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `chargeType` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `closeDate` | Date Closed | string | date |  |  |  |
| `commitInventory` |  | object |  |  |  |  |
| `commitInventory.id` | Internal identifier | string |  |  |  | `1`, `2`, `3` |
| `commitInventory.refName` | Reference Name | string |  |  |  |  |
| `commitmentFirm` | Commitment Confirmed | boolean |  |  |  |  |
| `costEstimate` | Est. Cost | number | double |  |  |  |
| `costEstimateRate` | Est. Rate | number | double |  |  |  |
| `costEstimateType` |  | object |  |  |  |  |
| `costEstimateType.id` | Internal identifier | string |  |  |  | `PREFVENDORRATE`, `AVGCOST`, `PURCHORDERRATE`, `LASTPURCHPRICE`, `MEMBERDEFINED`, `CUSTOM`, `ITEMDEFINED`, `PURCHPRICE` |
| `costEstimateType.refName` | Reference Name | string |  |  |  |  |
| `createPo` |  | object |  |  |  |  |
| `createPo.id` | Internal identifier | string |  |  |  | `CostRtrn`, `EndrTeg`, `SpecOrd`, `AuthDep`, `InTrnPay`, `POrdBlnk`, `ResvShip`, `Capture`, `GLAdj`, `OppClose`, `LandCost`, `CountAdj`, `OrdReval`, `Unbuild`, `IntcoAdj`, `CpFxVar`, `OrdAlloc`, `FxAsset`, `GACAdjst`, `WaveShip`, `RfqCtrct`, `POrdPrep`, `OwnRcpt`, `Transfrm`, `DepRfnd`, `BillVar`, `OrdBuild`, `FftRqFt`, `DepAppl`, `Payment`, `Refund`, `ColTeg`, `Reimb`, `OrdDgrss`, `KitShip`, `OrdAuth`, `WipBuild`, `CtrctOrd`, `OrdClose`, `RevRec`, `OrdRvCom`, `PickPack`, `TOrdCost`, `SysJrnl`, `Commissn`, `COGS`, `SrcContr`, `OsrcMfg`, `EstInvc`, `RfqVend`, `OrdDep`, `WOReval`, `CostRec`, `PurchOwn`, `OppEst`, `POrdReq`, `OrdBill`, `ExpRec`, `NetAsset`, `PrepAppl`, `OrdFftRq`, `BillRcpt`, `OrdArrng`, `PurchRet`, `CostDef`, `ShipRcpt`, `SaleRet`, `DiscTeg`, `RcptBill`, `CostDefR`, `DropShip`, `WaveOrd`, `PayTeg` |
| `createPo.refName` | Reference Name | string |  |  |  |  |
| `createWo` | Create WO | boolean |  |  |  |  |
| `createdPo` |  | purchaseOrder |  |  | [`purchaseOrder`](purchaseOrder.md#purchaseorder) |  |
| `daysLate` | Days Late | integer | int64 |  |  |  |
| `deferRevRec` | Deferred Revenue | boolean |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `doNotCreateRevenueElement` | Do Not Create Revenue Element | boolean |  |  |  |  |
| `estGrossProfit` | Est. Gross Profit | number | double |  |  |  |
| `estGrossProfitPercent` | Est. Gross Profit Percent | number | double |  |  |  |
| `excludeFromPredictiveRisk` | Exclude From Predictive Risk | boolean |  |  |  |  |
| `excludeFromRateRequest` | Exclude Item from Rate Request | boolean |  |  |  |  |
| `expectedShipDate` | Expected Ship Date | string | date |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `fromJob` | From Project | boolean |  |  |  |  |
| `giftCertFrom` | From | string |  |  |  |  |
| `giftCertMessage` | Gift Message | string |  |  |  |  |
| `giftCertNumber` | Code | string |  |  |  |  |
| `giftCertRecipientEmail` | Recipient Email | string |  |  |  |  |
| `giftCertRecipientName` | Recipient Name | string |  |  |  |  |
| `grossAmt` | Gross Amount | number | double |  |  |  |
| `hasOrdBillLink` | Has Order Billing link | boolean |  |  |  |  |
| `initOqpBucket` | Initial OQP Bucket | string |  |  |  |  |
| `inventoryDetail` |  | salesOrder-item-inventoryDetail |  |  | [`salesOrder-item-inventoryDetail`](#salesorder-item-inventorydetail) |  |
| `inventorylocation` |  | location |  |  | [`location`](location.md#location) |  |
| `inventorysubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `isAllocateFirmInvtOnly` | None | boolean |  |  |  |  |
| `isCatchWeightItem` |  | boolean |  |  |  |  |
| `isClosed` | Closed | boolean |  |  |  |  |
| `isEstimate` | Estimate | boolean |  |  |  |  |
| `isFreezeFirmAllocation` | None | boolean |  |  |  |  |
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
| `lastPurchasePrice` | Last Purchase Price | number | double |  |  |  |
| `licenseCode` | License Code | string |  |  |  |  |
| `line` | Transaction Line | integer | int64 |  |  |  |
| `lineUniqueKey` | Line Unique Key | string |  |  |  |  |
| `linked` | Linked | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `locationAutoAssigned` | Location Auto Assigned | boolean |  |  |  |  |
| `marginal` | Marginal | boolean |  |  |  |  |
| `matrixType` | Matrix Type | string |  |  |  |  |
| `minQty` | Minimum Quantity | number | float |  |  |  |
| `netAltSalesAmt` | Net Alt. Sales Amount | number | double |  |  |  |
| `noAutoAssignLocation` | Do Not Auto Assign Location | boolean |  |  |  |  |
| `options` | Options | string |  |  |  |  |
| `oqpBucket` | Oqp Bucket | string |  |  |  |  |
| `orderAllocationStrategy` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `orderPriority` | Order Priority | number | float |  |  |  |
| `poCurrency` | Currency | string |  |  |  |  |
| `poRate` | PO Rate | number | double |  |  |  |
| `poVendor` |  | vendor |  |  | [`vendor`](vendor.md#vendor) |  |
| `price` |  | priceLevel |  |  | [`priceLevel`](priceLevel.md#pricelevel) |  |
| `priceIntervalFrequency` |  | string |  |  |  |  |
| `priceIntervalFrequencyName` | Subscription Frequency | string |  |  |  |  |
| `priceIntervalRepeatEvery` | Subscription Frequency Repeat Every | string |  |  |  |  |
| `primaryToSecondaryUnitConversionRate` |  | number | float |  |  |  |
| `printItems` | Print Items | boolean |  |  |  |  |
| `processedByRevCommit` | Processed by Rev Commit | boolean |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityAllocated` | Quantity Allocated | number | float |  |  |  |
| `quantityAvailable` | Available | number | float |  |  |  |
| `quantityBackOrdered` | Back Ordered | number | float |  |  |  |
| `quantityBilled` | Invoiced | number | float |  |  |  |
| `quantityCommitted` | Committed | number | float |  |  |  |
| `quantityDemandAllocated` | Allocated Demand | number | float |  |  |  |
| `quantityFulfilled` | Quantity Fulfilled | number | float |  |  |  |
| `quantityOnHand` | On Hand | number | float |  |  |  |
| `quantityOrdered` | Quantity Ordered | number | float |  |  |  |
| `quantityPacked` | Quantity Packed | number | float |  |  |  |
| `quantityPicked` | Quantity Picked | number | float |  |  |  |
| `quantityReceived` | Quantity Received | number | float |  |  |  |
| `rate` | Rate | number | double |  |  |  |
| `rateIncludingTax` | Rate | number | double |  |  |  |
| `rateSchedule` | Rate Schedule | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `requestedDate` | Requested Date | string | date |  |  |  |
| `requiredDepositAmount` | Required Deposit Amount | number | double |  |  |  |
| `revRecEndDate` | Rev. Rec. End Date | string | date |  |  |  |
| `revRecSchedule` |  | revRecSchedule |  |  | [`revRecSchedule`](revRecSchedule.md#revrecschedule) |  |
| `revRecStartDate` | Rev. Rec. Start Date | string | date |  |  |  |
| `revRecTermInMonths` | Rev. Rec. Term in Months | integer | int64 |  |  |  |
| `revrec_recurrencetype` | Rev Rec Recurrence Type | string |  |  |  |  |
| `secondaryQuantity` | Secondary Quantity | number | float |  |  |  |
| `secondaryUnitConversionRate` |  | number | float |  |  |  |
| `secondaryUnits` | Secondary Units | string |  |  |  |  |
| `secondaryUnitsList` |  | string |  |  |  |  |
| `serialNumbers` | Serial/Lot Numbers | string |  |  |  |  |
| `shipAddress` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `shipCarrier` |  | object |  |  |  |  |
| `shipCarrier.id` | Internal identifier | string |  |  |  | `ups`, `nonups` |
| `shipCarrier.refName` | Reference Name | string |  |  |  |  |
| `shipGroup` | Ship Group | integer | int64 |  |  |  |
| `shipMethod` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
| `subscription` |  | subscription |  |  | [`subscription`](subscription.md#subscription) |  |
| `subscriptionLine` |  | subscriptionLine |  |  | [`subscriptionLine`](subscriptionLine.md#subscriptionline) |  |
| `subscriptionLinePeriodAmount` | Subscription Amount Per Period | number | double |  |  |  |
| `subscriptionLineRate` | Subscription Rate | number | double |  |  |  |
| `subscriptionLineType` |  | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tax1Amt` | Tax Amount | number | double |  |  |  |
| `taxAmount` | Tax Amount | number | double |  |  |  |
| `taxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxDetailsReference` | Tax Details Reference | string |  |  |  |  |
| `taxRate1` | Tax Rate | number | double |  |  |  |
| `taxRate2` | PST | number | double |  |  |  |
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
| `woId` | Work Order ID | string |  |  |  |  |

## salesOrder-partnersCollection

Browser definition `salesOrder-partnersCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesOrder-partnersElement[] |  |  | [`salesOrder-partnersElement`](#salesorder-partnerselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesOrder-partnersElement

Browser definition `salesOrder-partnersElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `contribution` | Contribution % | number | double |  |  |  |
| `isPrimary` | Primary | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `partner` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `partnerRole` |  | partnerCategory |  |  | [`partnerCategory`](partnerCategory.md#partnercategory) |  |
| `refName` | Reference Name | string |  |  |  |  |

## salesOrder-promotionsCollection

Browser definition `salesOrder-promotionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesOrder-promotionsElement[] |  |  | [`salesOrder-promotionsElement`](#salesorder-promotionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesOrder-promotionsElement

Browser definition `salesOrder-promotionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `couponCode` |  | couponCode |  |  | [`couponCode`](couponCode.md#couponcode) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `promoCode` |  | promotionCode |  |  | [`promotionCode`](promotionCode.md#promotioncode) |  |
| `refName` | Reference Name | string |  |  |  |  |

## salesOrder-salesTeamCollection

Browser definition `salesOrder-salesTeamCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesOrder-salesTeamElement[] |  |  | [`salesOrder-salesTeamElement`](#salesorder-salesteamelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesOrder-salesTeamElement

Browser definition `salesOrder-salesTeamElement`.

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

## salesOrder-shipGroupCollection

Browser definition `salesOrder-shipGroupCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesOrder-shipGroupElement[] |  |  | [`salesOrder-shipGroupElement`](#salesorder-shipgroupelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesOrder-shipGroupElement

Browser definition `salesOrder-shipGroupElement`.

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

## salesOrder-shippingAddress

Browser definition `salesOrder-shippingAddress`.

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

## salesOrder-taxDetailsCollection

Browser definition `salesOrder-taxDetailsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | salesOrder-taxDetailsElement[] |  |  | [`salesOrder-taxDetailsElement`](#salesorder-taxdetailselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesOrder-taxDetailsElement

Browser definition `salesOrder-taxDetailsElement`.

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

## salesOrderCollection

Browser definition `salesOrderCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | salesOrder[] |  |  | [`salesOrder`](#salesorder) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesOrderSelectOptions

Browser definition `salesOrderSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `alaConfiguration` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billAddressList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billCountry` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
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
| `drAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entityTaxRegNum` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `fxAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `groupedTo` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `handlingMode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `handlingTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `intercoStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `intercoTransaction` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `job` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `leadSource` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `messageSel` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nexus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `opportunity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `orderStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `orderType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `partner` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentOperation` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentOption` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentProcessingProfile` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
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
| `sourceWebSite` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiaryTaxRegNum` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `terms` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transactionToRefund` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

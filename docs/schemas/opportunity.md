# Schemas: opportunity

Property tables for definitions owned by `opportunity`.

Record page: [opportunity](../records/opportunity.md).

## Index

- [opportunity](#opportunity) — 132 properties
- [opportunity-accountingBookDetailCollection](#opportunity-accountingbookdetailcollection) — 6 properties
- [opportunity-accountingBookDetailElement](#opportunity-accountingbookdetailelement) — 7 properties
- [opportunity-appliedRulesCollection](#opportunity-appliedrulescollection) — 6 properties
- [opportunity-appliedRulesElement](#opportunity-appliedruleselement) — 9 properties
- [opportunity-billingAddress](#opportunity-billingaddress) — 18 properties
- [opportunity-competitorsCollection](#opportunity-competitorscollection) — 6 properties
- [opportunity-competitorsElement](#opportunity-competitorselement) — 7 properties
- [opportunity-estimatesCollection](#opportunity-estimatescollection) — 6 properties
- [opportunity-estimatesElement](#opportunity-estimateselement) — 12 properties
- [opportunity-itemCollection](#opportunity-itemcollection) — 6 properties
- [opportunity-itemElement](#opportunity-itemelement) — 71 properties
- [opportunity-partnersCollection](#opportunity-partnerscollection) — 6 properties
- [opportunity-partnersElement](#opportunity-partnerselement) — 6 properties
- [opportunity-salesTeamCollection](#opportunity-salesteamcollection) — 6 properties
- [opportunity-salesTeamElement](#opportunity-salesteamelement) — 8 properties
- [opportunity-shippingAddress](#opportunity-shippingaddress) — 18 properties
- [opportunity-taxDetailsCollection](#opportunity-taxdetailscollection) — 6 properties
- [opportunity-taxDetailsElement](#opportunity-taxdetailselement) — 14 properties
- [opportunityCollection](#opportunitycollection) — 6 properties
- [opportunitySelectOptions](#opportunityselectoptions) — 31 properties

## opportunity

Browser definition `opportunity`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBookDetail` |  | opportunity-accountingBookDetailCollection |  |  | [`opportunity-accountingBookDetailCollection`](#opportunity-accountingbookdetailcollection) |  |
| `actionItem` | Action Item | string |  |  |  |  |
| `altSalesRangeHigh` | Alt. Sales Range High | number | double |  |  |  |
| `altSalesRangeLow` | Alt. Sales Range Low | number | double |  |  |  |
| `altSalesTotal` | Alt. Sales Total | number | double |  |  |  |
| `appliedRules` |  | opportunity-appliedRulesCollection |  |  | [`opportunity-appliedRulesCollection`](#opportunity-appliedrulescollection) |  |
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
| `billingAddress` |  | opportunity-billingAddress |  |  | [`opportunity-billingAddress`](#opportunity-billingaddress) |  |
| `billingAddress_text` | Billing Address | string |  |  |  |  |
| `buyingReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `buyingTimeFrame` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `canHaveStackable` | Can Stack Promotions | boolean |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `closeDate` | Actual Close | string | date |  |  |  |
| `competitors` |  | opportunity-competitorsCollection |  |  | [`opportunity-competitorsCollection`](#opportunity-competitorscollection) |  |
| `contribPct` | Contribution Percentage | string |  |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `daysOpen` | Days Open | integer | int64 |  |  |  |
| `daysOverdueSearch` | Days Overdue | integer | int64 |  |  |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `entityStatus` |  | customerStatus |  |  | [`customerStatus`](customerStatus.md#customerstatus) |  |
| `entityTaxRegNum` | Customer Tax Reg. Number | string |  |  |  |  |
| `estGrossProfit` | Est. Gross Profit | number | double |  |  |  |
| `estGrossProfitPercent` | Est. Gross Profit Percent | number | double |  |  |  |
| `estimatedBudget` | Estimated Budget | number | double |  |  |  |
| `estimates` |  | opportunity-estimatesCollection |  |  | [`opportunity-estimatesCollection`](#opportunity-estimatescollection) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `excludeCommission` | Exclude Commissions | boolean |  |  |  |  |
| `expectedCloseDate` | Expected Close Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `forecastType` |  | object |  |  |  |  |
| `forecastType.id` | Internal identifier | string |  |  |  | `0`, `1`, `2`, `3` |
| `forecastType.refName` | Reference Name | string |  |  |  |  |
| `fxAltSalesTotal` | Foreign Alt. Sales Total | number | double |  |  |  |
| `fxNetAltSalesTotal` | Foreign Net Alt. Sales Total | number | double |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isBudgetApproved` | Budget Approved | boolean |  |  |  |  |
| `isTaxable` | Taxable | boolean |  |  |  |  |
| `item` |  | opportunity-itemCollection |  |  | [`opportunity-itemCollection`](#opportunity-itemcollection) |  |
| `job` |  | job |  |  | [`job`](job.md#job) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `leadSource` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Details | string |  |  |  |  |
| `netAltSalesTotal` | Net Alt. Sales Total | number | double |  |  |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `oneTime` | One Time | number | double |  |  |  |
| `originator` | Originator | string |  |  |  |  |
| `partner` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `partners` |  | opportunity-partnersCollection |  |  | [`opportunity-partnersCollection`](#opportunity-partnerscollection) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `prevPartner` | Previous Partner | integer | int64 |  |  |  |
| `prevRep` | Previous Representative | integer | int64 |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `probability` | Probability (%) | number | double |  |  |  |
| `projAltSalesAmt` | Projected Alt. Sales Amount | number | double |  |  |  |
| `projectedTotal` | Projected Total | number | double |  |  |  |
| `rangeHigh` | Range High | number | double |  |  |  |
| `rangeLow` | Range Low | number | double |  |  |  |
| `recurAnnually` | Annually | number | double |  |  |  |
| `recurMonthly` | Monthly | number | double |  |  |  |
| `recurQuarterly` | Quarterly | number | double |  |  |  |
| `recurWeekly` | Weekly | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `refreshFromSubscription` |  | string |  |  |  |  |
| `salesChannel` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `salesEffectiveDate` | Sales Effective Date | string | date |  |  |  |
| `salesGroup` |  | entityGroup |  |  | [`entityGroup`](entityGroup.md#entitygroup) |  |
| `salesReadiness` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `salesRep` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `salesTeam` |  | opportunity-salesTeamCollection |  |  | [`opportunity-salesTeamCollection`](#opportunity-salesteamcollection) |  |
| `saleschannelorderpriority` |  | string |  |  |  |  |
| `shipAddress` | Ship To | string |  |  |  |  |
| `shipAddressList` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `shipIsResidential` | Shipping address is residential | boolean |  |  |  |  |
| `shipOverride` | Override | boolean |  |  |  |  |
| `shippingAddress` |  | opportunity-shippingAddress |  |  | [`opportunity-shippingAddress`](#opportunity-shippingaddress) |  |
| `shippingAddress_text` | Shipping Address | string |  |  |  |  |
| `source` |  | object |  |  |  |  |
| `source.id` | Internal identifier | string |  |  |  | `SuitePhone`, `smbXML`, `CSV`, `ADP`, `QIF`, `QB`, `PERQUEST`, `Yahoo`, `PaymentLink`, `customerCenter`, `webServices`, `eBay`, `restWebServices`, `NLWebStore`, `offlineClient`, `SCIS`, `Sync` |
| `source.refName` | Reference Name | string |  |  |  |  |
| `sourceSystem` |  | object |  |  |  |  |
| `sourceSystem.id` | Internal identifier | string |  |  |  | `SuitePhone`, `smbXML`, `CSV`, `ADP`, `QIF`, `QB`, `PERQUEST`, `Yahoo`, `PaymentLink`, `customerCenter`, `webServices`, `eBay`, `restWebServices`, `NLWebStore`, `offlineClient`, `SCIS`, `Sync` |
| `sourceSystem.refName` | Reference Name | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `A`, `B`, `C`, `D` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `storeOrder` |  | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `subsidiaryTaxRegNum` | Subsidiary Tax Reg. Number | string |  |  |  |  |
| `syncPartnerTeams` | Update Customer | boolean |  |  |  |  |
| `syncSalesTeams` | Update Customer | boolean |  |  |  |  |
| `tax2Total` | PST | number | double |  |  |  |
| `taxDetails` |  | opportunity-taxDetailsCollection |  |  | [`opportunity-taxDetailsCollection`](#opportunity-taxdetailscollection) |  |
| `taxDetailsOverride` | Tax Details Override | boolean |  |  |  |  |
| `taxItem` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxPointDate` | Tax Point Date | string | date |  |  |  |
| `taxPointDateOverride` | Tax Point Date Override | boolean |  |  |  |  |
| `taxRate` | Tax Rate | number | float |  |  |  |
| `taxRegOverride` | Tax Registration Override | boolean |  |  |  |  |
| `taxTotal` | Tax Total | number | double |  |  |  |
| `title` | Title | string |  |  |  |  |
| `total` | Total | number | double |  |  |  |
| `totalAfterTaxes` | Total After Taxes | number | double |  |  |  |
| `totalCostEstimate` | Est. Cost | number | double |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Opportunity # | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `vatRegNum` | VAT Registration | string |  |  |  |  |
| `webSite` |  | string |  |  |  |  |
| `weightedTotal` | Weighted Total | number | double |  |  |  |
| `winLossReason` |  | winLossReason |  |  | [`winLossReason`](winLossReason.md#winlossreason) |  |

## opportunity-accountingBookDetailCollection

Browser definition `opportunity-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | opportunity-accountingBookDetailElement[] |  |  | [`opportunity-accountingBookDetailElement`](#opportunity-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## opportunity-accountingBookDetailElement

Browser definition `opportunity-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## opportunity-appliedRulesCollection

Browser definition `opportunity-appliedRulesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | opportunity-appliedRulesElement[] |  |  | [`opportunity-appliedRulesElement`](#opportunity-appliedruleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## opportunity-appliedRulesElement

Browser definition `opportunity-appliedRulesElement`.

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

## opportunity-billingAddress

Browser definition `opportunity-billingAddress`.

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

## opportunity-competitorsCollection

Browser definition `opportunity-competitorsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | opportunity-competitorsElement[] |  |  | [`opportunity-competitorsElement`](#opportunity-competitorselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## opportunity-competitorsElement

Browser definition `opportunity-competitorsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `competitor` |  | competitor |  |  | [`competitor`](competitor.md#competitor) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `notes` | Notes | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `strategy` | Strategy | string |  |  |  |  |
| `url` | URL | string |  |  |  |  |
| `winner` | Winner | boolean |  |  |  |  |

## opportunity-estimatesCollection

Browser definition `opportunity-estimatesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | opportunity-estimatesElement[] |  |  | [`opportunity-estimatesElement`](#opportunity-estimateselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## opportunity-estimatesElement

Browser definition `opportunity-estimatesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `expectedCloseDate` | Exp. Close Date | string | date |  |  |  |
| `forecastType` |  | object |  |  |  |  |
| `forecastType.id` | Internal identifier | string |  |  |  | `0`, `1`, `2`, `3` |
| `forecastType.refName` | Reference Name | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `probability` | Probability | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `status` | Status | string |  |  |  |  |
| `title` | Title | string |  |  |  |  |
| `total` | Amount | number | double |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Number | string |  |  |  |  |

## opportunity-itemCollection

Browser definition `opportunity-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | opportunity-itemElement[] |  |  | [`opportunity-itemElement`](#opportunity-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## opportunity-itemElement

Browser definition `opportunity-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `altSalesAmt` | Alt. Sales Amount | number | double |  |  |  |
| `amount` | Amount | number | double |  |  |  |
| `baseGrossAmt` | Gross Amount | number | double |  |  |  |
| `billVarianceStatus` |  | object |  |  |  |  |
| `billVarianceStatus.id` | Internal identifier | string |  |  |  | `NOVARIANCES`, `JOURNALNOTPOSTED`, `JOURNALPOSTED` |
| `billVarianceStatus.refName` | Reference Name | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `costEstimate` | Est. Cost | number | double |  |  |  |
| `costEstimateRate` | Est. Rate | number | double |  |  |  |
| `costEstimateType` |  | object |  |  |  |  |
| `costEstimateType.id` | Internal identifier | string |  |  |  | `PREFVENDORRATE`, `AVGCOST`, `PURCHORDERRATE`, `LASTPURCHPRICE`, `MEMBERDEFINED`, `CUSTOM`, `ITEMDEFINED`, `PURCHPRICE` |
| `costEstimateType.refName` | Reference Name | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `estGrossProfit` | Est. Gross Profit | number | double |  |  |  |
| `estGrossProfitPercent` | Est. Gross Profit Percent | number | double |  |  |  |
| `expectedShipDate` | Expected Ship Date | string | date |  |  |  |
| `fromJob` | From Project | boolean |  |  |  |  |
| `grossAmt` | Gross Amount | number | double |  |  |  |
| `initOqpBucket` | Initial OQP Bucket | string |  |  |  |  |
| `isClosed` | Closed | boolean |  |  |  |  |
| `isEstimate` | Estimate | boolean |  |  |  |  |
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
| `netAltSalesAmt` | Net Alt. Sales Amount | number | double |  |  |  |
| `options` | Options | string |  |  |  |  |
| `oqpBucket` | Oqp Bucket | string |  |  |  |  |
| `price` |  | priceLevel |  |  | [`priceLevel`](priceLevel.md#pricelevel) |  |
| `priceIntervalFrequency` |  | string |  |  |  |  |
| `priceIntervalFrequencyName` | Subscription Frequency | string |  |  |  |  |
| `priceIntervalRepeatEvery` | Subscription Frequency Repeat Every | string |  |  |  |  |
| `printItems` | Print Items | boolean |  |  |  |  |
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

## opportunity-partnersCollection

Browser definition `opportunity-partnersCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | opportunity-partnersElement[] |  |  | [`opportunity-partnersElement`](#opportunity-partnerselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## opportunity-partnersElement

Browser definition `opportunity-partnersElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `contribution` | Contribution % | number | double |  |  |  |
| `isPrimary` | Primary | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `partner` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `partnerRole` |  | partnerCategory |  |  | [`partnerCategory`](partnerCategory.md#partnercategory) |  |
| `refName` | Reference Name | string |  |  |  |  |

## opportunity-salesTeamCollection

Browser definition `opportunity-salesTeamCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | opportunity-salesTeamElement[] |  |  | [`opportunity-salesTeamElement`](#opportunity-salesteamelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## opportunity-salesTeamElement

Browser definition `opportunity-salesTeamElement`.

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

## opportunity-shippingAddress

Browser definition `opportunity-shippingAddress`.

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

## opportunity-taxDetailsCollection

Browser definition `opportunity-taxDetailsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | opportunity-taxDetailsElement[] |  |  | [`opportunity-taxDetailsElement`](#opportunity-taxdetailselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## opportunity-taxDetailsElement

Browser definition `opportunity-taxDetailsElement`.

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

## opportunityCollection

Browser definition `opportunityCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | opportunity[] |  |  | [`opportunity`](#opportunity) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## opportunitySelectOptions

Browser definition `opportunitySelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billAddressList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billCountry` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `buyingReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `buyingTimeFrame` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entityStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entityTaxRegNum` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `forecastType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `job` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `leadSource` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nexus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `partner` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesChannel` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesReadiness` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesRep` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipAddressList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `source` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceSystem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiaryTaxRegNum` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `winLossReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

# Schemas: customer

Property tables for definitions owned by `customer`.

Record page: [customer](../records/customer.md).

## Index

- [customer](#customer) — 184 properties
- [customer-addressBook-addressBookAddress](#customer-addressbook-addressbookaddress) — 18 properties
- [customer-addressBookCollection](#customer-addressbookcollection) — 6 properties
- [customer-addressBookElement](#customer-addressbookelement) — 12 properties
- [customer-campaignsCollection](#customer-campaignscollection) — 6 properties
- [customer-campaignsElement](#customer-campaignselement) — 2 properties
- [customer-contactRolesCollection](#customer-contactrolescollection) — 6 properties
- [customer-contactRolesElement](#customer-contactroleselement) — 9 properties
- [customer-currencyListCollection](#customer-currencylistcollection) — 6 properties
- [customer-currencyListElement](#customer-currencylistelement) — 16 properties
- [customer-groupPricingCollection](#customer-grouppricingcollection) — 6 properties
- [customer-groupPricingElement](#customer-grouppricingelement) — 4 properties
- [customer-itemPricingCollection](#customer-itempricingcollection) — 6 properties
- [customer-itemPricingElement](#customer-itempricingelement) — 6 properties
- [customer-partnersCollection](#customer-partnerscollection) — 6 properties
- [customer-partnersElement](#customer-partnerselement) — 7 properties
- [customer-salesTeamCollection](#customer-salesteamcollection) — 6 properties
- [customer-salesTeamElement](#customer-salesteamelement) — 7 properties
- [customer-subscriptionMessageHistoryCollection](#customer-subscriptionmessagehistorycollection) — 6 properties
- [customer-subscriptionMessageHistoryElement](#customer-subscriptionmessagehistoryelement) — 2 properties
- [customer-subscriptionsCollection](#customer-subscriptionscollection) — 6 properties
- [customer-subscriptionsElement](#customer-subscriptionselement) — 5 properties
- [customer-taxRegistrationCollection](#customer-taxregistrationcollection) — 6 properties
- [customer-taxRegistrationElement](#customer-taxregistrationelement) — 10 properties
- [customerCollection](#customercollection) — 6 properties
- [customerSelectOptions](#customerselectoptions) — 53 properties

## customer

Browser definition `customer`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accessRole` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `accountNumber` | Account | string |  |  |  |  |
| `acquisitionDate` | Acquisition Date | string | date |  |  |  |
| `addressBook` |  | customer-addressBookCollection |  |  | [`customer-addressBookCollection`](#customer-addressbookcollection) |  |
| `aging` | Current | number | double |  |  |  |
| `aging1` | 1-30 Days | number | double |  |  |  |
| `aging2` | 31-60 Days | number | double |  |  |  |
| `aging3` | 61-90 Days | number | double |  |  |  |
| `aging4` | Over 90 Days | number | double |  |  |  |
| `alcoholRecipientType` |  | object |  |  |  |  |
| `alcoholRecipientType.id` | Internal identifier | string |  |  |  | `CONSUMER`, `LICENSEE` |
| `alcoholRecipientType.refName` | Reference Name | string |  |  |  |  |
| `altEmail` | Alt. Email | string |  |  |  |  |
| `altName` | Customer | string |  |  |  |  |
| `altPhone` | Alt. Phone | string |  |  |  |  |
| `assignedWebSite` |  | webSite |  |  | [`webSite`](webSite.md#website) |  |
| `autoName` | Auto | boolean |  |  |  |  |
| `balance` | Balance | number | double |  |  |  |
| `billingRateCard` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `billingSchedule` |  | billingSchedule |  |  | [`billingSchedule`](billingSchedule.md#billingschedule) |  |
| `billingTransactionForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `billingTransactionType` |  | object |  |  |  |  |
| `billingTransactionType.id` | Internal identifier | string |  |  |  | `CashSale`, `CustInvc` |
| `billingTransactionType.refName` | Reference Name | string |  |  |  |  |
| `buyingReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `buyingTimeFrame` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `campaignCategory` |  | campaignCategory |  |  | [`campaignCategory`](campaignCategory.md#campaigncategory) |  |
| `campaignEvent` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `campaigns` |  | customer-campaignsCollection |  |  | [`customer-campaignsCollection`](#customer-campaignscollection) |  |
| `category` |  | customerCategory |  |  | [`customerCategory`](customerCategory.md#customercategory) |  |
| `clickStream` | Click-Stream (1st Visit) | string |  |  |  |  |
| `comments` | Comments | string |  |  |  |  |
| `companyName` | Company Name | string |  |  |  |  |
| `consolAging` | Consolidated Current | number | double |  |  |  |
| `consolAging1` | 1-30 Days | number | double |  |  |  |
| `consolAging2` | 31-60 Days | number | double |  |  |  |
| `consolAging3` | 61-90 Days | number | double |  |  |  |
| `consolAging4` | Over 90 Days | number | double |  |  |  |
| `consolBalance` | Consolidated | number | double |  |  |  |
| `consolDaysOverdue` | Consolidated | integer | int64 |  |  |  |
| `consolDepositBalance` | Consolidated | number | double |  |  |  |
| `consolOverdueBalance` | Consolidated | number | double |  |  |  |
| `consolUnbilledOrders` | Consolidated | number | double |  |  |  |
| `contact` |  | contact |  |  | [`contact`](contact.md#contact) |  |
| `contactList` |  | contactCollection |  |  | [`contactCollection`](contact.md#contactcollection) |  |
| `contactRoles` |  | customer-contactRolesCollection |  |  | [`customer-contactRolesCollection`](#customer-contactrolescollection) |  |
| `contribPct` | Contribution Percentage | string |  |  |  |  |
| `creditHoldOverride` |  | object |  |  |  |  |
| `creditHoldOverride.id` | Internal identifier | string |  |  |  | `AUTO`, `OFF`, `ON` |
| `creditHoldOverride.refName` | Reference Name | string |  |  |  |  |
| `creditLimit` | Credit Limit | number | double |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `currencyList` |  | customer-currencyListCollection |  |  | [`customer-currencyListCollection`](#customer-currencylistcollection) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `dateCreated` | Date Created | string | date-time |  |  |  |
| `daysOverdue` | Days | integer | int64 |  |  |  |
| `defaultAddress` | Default Address | string |  |  |  |  |
| `defaultAllocationStrategy` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `defaultBankAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `defaultOrderPriority` | Default Order Priority | number | float |  |  |  |
| `defaultShippingAddress` | Default Shipping Address | string |  |  |  |  |
| `defaultTaxReg` | Default Tax Reg. Number | string |  |  |  |  |
| `depositBalance` | Deposit Balance | number | double |  |  |  |
| `displaySymbol` | Currency Symbol | string |  |  |  |  |
| `drAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `email` | Email | string |  |  |  |  |
| `emailPreference` |  | object |  |  |  |  |
| `emailPreference.id` | Internal identifier | string |  |  |  | `PDF`, `HTML`, `DEFAULT` |
| `emailPreference.refName` | Reference Name | string |  |  |  |  |
| `emailTransactions` | Email Transactions | boolean |  |  |  |  |
| `endDate` | End Date | string | date |  |  |  |
| `entityId` | Entity ID | string |  |  |  |  |
| `entityStatus` |  | customerStatus |  |  | [`customerStatus`](customerStatus.md#customerstatus) |  |
| `estimatedBudget` | Estimated Budget | number | double |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fax` | Fax | string |  |  |  |  |
| `faxTransactions` | Fax Transactions | boolean |  |  |  |  |
| `firstName` | First Name | string |  |  |  |  |
| `firstOrderDate` | First Sales Order Date | string | date |  |  |  |
| `firstSaleDate` | First Sale Date | string | date |  |  |  |
| `firstVisit` | First Visit | string | date-time |  |  |  |
| `fxAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `giveAccess` | Login Access | boolean |  |  |  |  |
| `globalSubscriptionStatus` |  | object |  |  |  |  |
| `globalSubscriptionStatus.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `globalSubscriptionStatus.refName` | Reference Name | string |  |  |  |  |
| `groupInvoices` | Group Invoices | boolean |  |  |  |  |
| `groupPricing` |  | customer-groupPricingCollection |  |  | [`customer-groupPricingCollection`](#customer-grouppricingcollection) |  |
| `homePhone` | Home Phone | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `image` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `isAutogeneratedRepresentingEntity` | Is Autogenerated Representing Entity | boolean |  |  |  |  |
| `isBudgetApproved` | Budget Approved | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isPerson` | Is Individual | boolean |  |  |  |  |
| `itemPricing` |  | customer-itemPricingCollection |  |  | [`customer-itemPricingCollection`](#customer-itempricingcollection) |  |
| `keywords` | Search Engine Keywords (1st Visit) | string |  |  |  |  |
| `language` |  | object |  |  |  |  |
| `language.id` | Internal identifier | string |  |  |  | `ro_RO`, `af_ZA`, `tl_PH`, `pt_BR`, `th_TH`, `bn_BD`, `cs_CZ`, `ca_ES`, `hu_HU`, `kn_IN`, `sk_SK`, `es_ES`, `nl_NL`, `te_IN`, `is_IS`, `sq_AL`, `sv_SE`, `es_AR`, `da_DK`, `ta_IN`, `sr_RS`, `en`, `ar`, `hr_HR`, `ko_KR`, `en_US`, `lt_LT`, `no_NO`, `it_IT`, `ru_RU`, `el_GR`, `pl_PL`, `en_AU`, `tr_TR`, `id_ID`, `hi_IN`, `mr_IN`, `ja_JP`, `fr_FR`, `he_IL`, `de_DE`, `ms_MY`, `zh_TW`, `fr_CA`, `pa_IN`, `fa_IR`, `bg_BG`, `vi_VN`, `hy_AM`, `lb_LU`, `sh_RS`, `ht_HT`, `fi_FI`, `en_GB`, `gu_IN`, `et_EE`, `en_CA`, `bs_BA`, `uk_UA`, `lv_LV`, `zh_CN`, `sl_SI`, `pt_PT` |
| `language.refName` | Reference Name | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `lastName` | Last Name | string |  |  |  |  |
| `lastOrderDate` | Last Sales Order Date | string | date |  |  |  |
| `lastPageVisited` | Last Page Visited | string |  |  |  |  |
| `lastSaleDate` | Last Sales Date | string | date |  |  |  |
| `lastVisit` | Last Visit | string | date-time |  |  |  |
| `leadSource` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `middleName` | Middle Name | string |  |  |  |  |
| `mobilePhone` | Mobile Phone | string |  |  |  |  |
| `monthlyClosing` |  | object |  |  |  |  |
| `monthlyClosing.id` | Internal identifier | string |  |  |  | `1`, `25`, `15`, `5`, `31`, `20`, `10` |
| `monthlyClosing.refName` | Reference Name | string |  |  |  |  |
| `negativeNumberFormat` |  | object |  |  |  |  |
| `negativeNumberFormat.id` | Internal identifier | string |  |  |  | `0`, `1` |
| `negativeNumberFormat.refName` | Reference Name | string |  |  |  |  |
| `numberFormat` |  | object |  |  |  |  |
| `numberFormat.id` | Internal identifier | string |  |  |  | `0`, `1`, `2`, `3`, `4`, `5` |
| `numberFormat.refName` | Reference Name | string |  |  |  |  |
| `openingBalance` | Opening Balance | number | double |  |  |  |
| `openingBalanceAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `openingBalanceDate` | Opening Balance Date | string | date |  |  |  |
| `overdueBalance` | Overdue | number | double |  |  |  |
| `overrideCurrencyFormat` | Override Currency Format | boolean |  |  |  |  |
| `parent` |  | customer |  |  | [`customer`](#customer) |  |
| `partner` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `partners` |  | customer-partnersCollection |  |  | [`customer-partnersCollection`](#customer-partnerscollection) |  |
| `password` | Password | string |  |  |  |  |
| `password2` | Confirm Password | string |  |  |  |  |
| `phone` | Phone | string |  |  |  |  |
| `phoneticName` | Furigana | string |  |  |  |  |
| `prefCcProcessor` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `priceLevel` |  | priceLevel |  |  | [`priceLevel`](priceLevel.md#pricelevel) |  |
| `printOnCheckAs` | Print on Check As | string |  |  |  |  |
| `printTransactions` | Print Transactions | boolean |  |  |  |  |
| `receivablesAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `referrer` | Referrer (1st Visit) | string |  |  |  |  |
| `reminderDays` | Reminder Days | integer | int64 |  |  |  |
| `representingSubsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `resaleNumber` | Resale Number | string |  |  |  |  |
| `salesGroup` |  | entityGroup |  |  | [`entityGroup`](entityGroup.md#entitygroup) |  |
| `salesReadiness` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `salesRep` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `salesTeam` |  | customer-salesTeamCollection |  |  | [`customer-salesTeamCollection`](#customer-salesteamcollection) |  |
| `salutation` | Mr./Ms... | string |  |  |  |  |
| `searchStage` | Stage | string |  |  |  |  |
| `sendEmail` | Send New Access Notification Email | boolean |  |  |  |  |
| `shipComplete` | Ship Complete | boolean |  |  |  |  |
| `shippingCarrier` |  | object |  |  |  |  |
| `shippingCarrier.id` | Internal identifier | string |  |  |  |  |
| `shippingCarrier.refName` | Reference Name | string |  |  |  |  |
| `shippingItem` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
| `sourceWebSite` |  | webSite |  |  | [`webSite`](webSite.md#website) |  |
| `startDate` | Start Date | string | date |  |  |  |
| `subscriptionMessageHistory` |  | customer-subscriptionMessageHistoryCollection |  |  | [`customer-subscriptionMessageHistoryCollection`](#customer-subscriptionmessagehistorycollection) |  |
| `subscriptions` |  | customer-subscriptionsCollection |  |  | [`customer-subscriptionsCollection`](#customer-subscriptionscollection) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `symbolPlacement` |  | object |  |  |  |  |
| `symbolPlacement.id` | Internal identifier | string |  |  |  | `1`, `2` |
| `symbolPlacement.refName` | Reference Name | string |  |  |  |  |
| `syncPartnerTeams` | Update Customer | boolean |  |  |  |  |
| `syncSalesTeams` | Update Customer | boolean |  |  |  |  |
| `taxExempt` | PST Exempt | boolean |  |  |  |  |
| `taxItem` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `taxRegistration` |  | customer-taxRegistrationCollection |  |  | [`customer-taxRegistrationCollection`](#customer-taxregistrationcollection) |  |
| `taxable` | Taxable | boolean |  |  |  |  |
| `terms` |  | term |  |  | [`term`](term.md#term) |  |
| `territory` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `thirdPartyAcct` | 3rd Party Billing Account Number | string |  |  |  |  |
| `thirdPartyCarrier` |  | object |  |  |  |  |
| `thirdPartyCarrier.id` | Internal identifier | string |  |  |  | `fedex`, `ups`, `usps` |
| `thirdPartyCarrier.refName` | Reference Name | string |  |  |  |  |
| `thirdPartyCountry` |  | object |  |  |  |  |
| `thirdPartyCountry.id` | Internal identifier | string |  |  |  | `PR`, `PS`, `PT`, `PW`, `PY`, `QA`, `AB`, `AD`, `AE`, `AF`, `AG`, `AI`, `AL`, `AM`, `AN`, `AO`, `AQ`, `AR`, `AS`, `AT`, `RE`, `AU`, `AW`, `AX`, `AZ`, `RO`, `BA`, `BB`, `RS`, `BD`, `BE`, `RU`, `BF`, `BG`, `RW`, `BH`, `BI`, `BJ`, `BL`, `BM`, `BN`, `BO`, `SA`, `BQ`, `SB`, `BR`, `SC`, `BS`, `SD`, `BT`, `SE`, `BV`, `SG`, `BW`, `SH`, `SI`, `BY`, `SJ`, `BZ`, `SK`, `SL`, `SM`, `SN`, `SO`, `CA`, `SR`, `CC`, `SS`, `CD`, `ST`, `CF`, `SV`, `CG`, `CH`, `SX`, `CI`, `SY`, `SZ`, `CK`, `CL`, `CM`, `CN`, `CO`, `CR`, `TC`, `CS`, `TD`, `CU`, `TF`, `CV`, `TG`, `CW`, `TH`, `CX`, `CY`, `TJ`, `CZ`, `TK`, `TL`, `TM`, `TN`, `TO`, `TR`, `TT`, `DE`, `TV`, `TW`, `DJ`, `TZ`, `DK`, `DM`, `DO`, `UA`, `UG`, `DZ`, `UM`, `EA`, `EC`, `US`, `EE`, `EG`, `EH`, `UY`, `UZ`, `VA`, `ER`, `VC`, `ES`, `ET`, `VE`, `VG`, `VI`, `VN`, `VU`, `FI`, `FJ`, `FK`, `FM`, `FO`, `FR`, `WF`, `GA`, `GB`, `WS`, `GD`, `GE`, `GF`, `GG`, `GH`, `GI`, `GL`, `GM`, `GN`, `GP`, `GQ`, `GR`, `GS`, `GT`, `GU`, `GW`, `GY`, `XK`, `HK`, `HM`, `HN`, `HR`, `HT`, `YE`, `HU`, `IC`, `ID`, `YT`, `IE`, `IL`, `IM`, `IN`, `IO`, `ZA`, `IQ`, `IR`, `IS`, `IT`, `ZM`, `JE`, `ZW`, `JM`, `JO`, `JP`, `KE`, `KG`, `KH`, `KI`, `KM`, `KN`, `KP`, `KR`, `KW`, `KY`, `KZ`, `LA`, `LB`, `LC`, `LI`, `LK`, `LR`, `LS`, `LT`, `LU`, `LV`, `LY`, `MA`, `MC`, `MD`, `ME`, `MF`, `MG`, `MH`, `MK`, `ML`, `MM`, `MN`, `MO`, `MP`, `MQ`, `MR`, `MS`, `MT`, `MU`, `MV`, `MW`, `MX`, `MY`, `MZ`, `NA`, `NC`, `NE`, `NF`, `NG`, `NI`, `NL`, `NO`, `NP`, `NR`, `NU`, `NZ`, `OM`, `PA`, `PE`, `PF`, `PG`, `PH`, `PK`, `PL`, `PM`, `PN` |
| `thirdPartyCountry.refName` | Reference Name | string |  |  |  |  |
| `thirdPartyZipCode` | 3rd Party Billing Zip | string |  |  |  |  |
| `title` | Job Title | string |  |  |  |  |
| `topLevelParent` |  | customer |  |  | [`customer`](#customer) |  |
| `unbilledOrders` | Unbilled Orders | number | double |  |  |  |
| `unsubscribe` | Unsubscribe from Campaigns | boolean |  |  |  |  |
| `url` | URL | string |  |  |  |  |
| `vatRegNumber` | VAT Registration No. | string |  |  |  |  |
| `visits` | Number of Visits | integer | int64 |  |  |  |

## customer-addressBook-addressBookAddress

Browser definition `customer-addressBook-addressBookAddress`.

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

## customer-addressBookCollection

Browser definition `customer-addressBookCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customer-addressBookElement[] |  |  | [`customer-addressBookElement`](#customer-addressbookelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customer-addressBookElement

Browser definition `customer-addressBookElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `addressBookAddress` |  | customer-addressBook-addressBookAddress |  |  | [`customer-addressBook-addressBookAddress`](#customer-addressbook-addressbookaddress) |  |
| `addressBookAddress_text` | Address | string |  |  |  |  |
| `addressId` | Internal ID | string |  |  |  |  |
| `defaultBilling` | Default Billing | boolean |  |  |  |  |
| `defaultShipping` | Default Shipping | boolean |  |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `isResidential` | Residential Address | boolean |  |  |  |  |
| `label` | Label | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## customer-campaignsCollection

Browser definition `customer-campaignsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customer-campaignsElement[] |  |  | [`customer-campaignsElement`](#customer-campaignselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customer-campaignsElement

Browser definition `customer-campaignsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## customer-contactRolesCollection

Browser definition `customer-contactRolesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customer-contactRolesElement[] |  |  | [`customer-contactRolesElement`](#customer-contactroleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customer-contactRolesElement

Browser definition `customer-contactRolesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `contact` |  | contact |  |  | [`contact`](contact.md#contact) |  |
| `contactName` | Contact | string |  |  |  |  |
| `email` | Email | string |  |  |  |  |
| `giveAccess` | Access | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `password` | Password | string |  |  |  |  |
| `passwordConfirm` | Confirm Password | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `role` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## customer-currencyListCollection

Browser definition `customer-currencyListCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customer-currencyListElement[] |  |  | [`customer-currencyListElement`](#customer-currencylistelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customer-currencyListElement

Browser definition `customer-currencyListElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `balance` | Balance | number | double |  |  |  |
| `consolBalance` | Consolidated Balance | number | double |  |  |  |
| `consolDepositBalance` | Consolidated Deposit Balance | number | double |  |  |  |
| `consolOverdueBalance` | Consolidated Overdue Balance | number | double |  |  |  |
| `consolUnbilledOrders` | Consolidated Unbilled Orders | number | double |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `depositBalance` | Deposit Balance | number | double |  |  |  |
| `displaySymbol` | Symbol | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `overdueBalance` | Overdue Balance | number | double |  |  |  |
| `overrideCurrencyFormat` | Override Currency Format | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `symbolPlacement` |  | object |  |  |  |  |
| `symbolPlacement.id` | Internal identifier | string |  |  |  | `1`, `2` |
| `symbolPlacement.refName` | Reference Name | string |  |  |  |  |
| `unbilledOrders` | Unbilled Orders | number | double |  |  |  |

## customer-groupPricingCollection

Browser definition `customer-groupPricingCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customer-groupPricingElement[] |  |  | [`customer-groupPricingElement`](#customer-grouppricingelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customer-groupPricingElement

Browser definition `customer-groupPricingElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `group` |  | pricingGroup |  |  | [`pricingGroup`](pricingGroup.md#pricinggroup) |  |
| `level` |  | priceLevel |  |  | [`priceLevel`](priceLevel.md#pricelevel) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## customer-itemPricingCollection

Browser definition `customer-itemPricingCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customer-itemPricingElement[] |  |  | [`customer-itemPricingElement`](#customer-itempricingelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customer-itemPricingElement

Browser definition `customer-itemPricingElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `level` |  | priceLevel |  |  | [`priceLevel`](priceLevel.md#pricelevel) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `price` | Unit Price | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## customer-partnersCollection

Browser definition `customer-partnersCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customer-partnersElement[] |  |  | [`customer-partnersElement`](#customer-partnerselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customer-partnersElement

Browser definition `customer-partnersElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `contribution` | Contribution % | number | double |  |  |  |
| `id` | ID | string |  |  |  |  |
| `isPrimary` | Primary | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `partner` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `partnerRole` |  | partnerCategory |  |  | [`partnerCategory`](partnerCategory.md#partnercategory) |  |
| `refName` | Reference Name | string |  |  |  |  |

## customer-salesTeamCollection

Browser definition `customer-salesTeamCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customer-salesTeamElement[] |  |  | [`customer-salesTeamElement`](#customer-salesteamelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customer-salesTeamElement

Browser definition `customer-salesTeamElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `contribution` | Contribution % | number | double |  |  |  |
| `employee` |  | employee |  |  | [`employee`](employee.md#employee) |  |
| `id` | ID | string |  |  |  |  |
| `isPrimary` | Primary | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `salesRole` |  | salesRole |  |  | [`salesRole`](salesRole.md#salesrole) |  |

## customer-subscriptionMessageHistoryCollection

Browser definition `customer-subscriptionMessageHistoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customer-subscriptionMessageHistoryElement[] |  |  | [`customer-subscriptionMessageHistoryElement`](#customer-subscriptionmessagehistoryelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customer-subscriptionMessageHistoryElement

Browser definition `customer-subscriptionMessageHistoryElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## customer-subscriptionsCollection

Browser definition `customer-subscriptionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customer-subscriptionsElement[] |  |  | [`customer-subscriptionsElement`](#customer-subscriptionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customer-subscriptionsElement

Browser definition `customer-subscriptionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `lastModifiedDate` | Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subscribed` | Subscribed | boolean |  |  |  |  |
| `subscription` |  | campaignSubscription |  |  | [`campaignSubscription`](campaignSubscription.md#campaignsubscription) |  |

## customer-taxRegistrationCollection

Browser definition `customer-taxRegistrationCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customer-taxRegistrationElement[] |  |  | [`customer-taxRegistrationElement`](#customer-taxregistrationelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customer-taxRegistrationElement

Browser definition `customer-taxRegistrationElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `address` | Address | string |  |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `nexusCountry` |  | object |  |  |  |  |
| `nexusCountry.id` | Internal identifier | string |  |  |  | `PR`, `PS`, `PT`, `PW`, `PY`, `QA`, `AB`, `AD`, `AE`, `AF`, `AG`, `AI`, `AL`, `AM`, `AN`, `AO`, `AQ`, `AR`, `AS`, `AT`, `RE`, `AU`, `AW`, `AX`, `AZ`, `RO`, `BA`, `BB`, `RS`, `BD`, `BE`, `RU`, `BF`, `BG`, `RW`, `BH`, `BI`, `BJ`, `BL`, `BM`, `BN`, `BO`, `SA`, `BQ`, `SB`, `BR`, `SC`, `BS`, `SD`, `BT`, `SE`, `BV`, `SG`, `BW`, `SH`, `SI`, `BY`, `SJ`, `BZ`, `SK`, `SL`, `SM`, `SN`, `SO`, `CA`, `SR`, `CC`, `SS`, `CD`, `ST`, `CF`, `SV`, `CG`, `CH`, `SX`, `CI`, `SY`, `SZ`, `CK`, `CL`, `CM`, `CN`, `CO`, `CR`, `TC`, `CS`, `TD`, `CU`, `TF`, `CV`, `TG`, `CW`, `TH`, `CX`, `CY`, `TJ`, `CZ`, `TK`, `TL`, `TM`, `TN`, `TO`, `TR`, `TT`, `DE`, `TV`, `TW`, `DJ`, `TZ`, `DK`, `DM`, `DO`, `UA`, `UG`, `DZ`, `UM`, `EA`, `EC`, `US`, `EE`, `EG`, `EH`, `UY`, `UZ`, `VA`, `ER`, `VC`, `ES`, `ET`, `VE`, `VG`, `VI`, `VN`, `VU`, `FI`, `FJ`, `FK`, `FM`, `FO`, `FR`, `WF`, `GA`, `GB`, `WS`, `GD`, `GE`, `GF`, `GG`, `GH`, `GI`, `GL`, `GM`, `GN`, `GP`, `GQ`, `GR`, `GS`, `GT`, `GU`, `GW`, `GY`, `XK`, `HK`, `HM`, `HN`, `HR`, `HT`, `YE`, `HU`, `IC`, `ID`, `YT`, `IE`, `IL`, `IM`, `IN`, `IO`, `ZA`, `IQ`, `IR`, `IS`, `IT`, `ZM`, `JE`, `ZW`, `JM`, `JO`, `JP`, `KE`, `KG`, `KH`, `KI`, `KM`, `KN`, `KP`, `KR`, `KW`, `KY`, `KZ`, `LA`, `LB`, `LC`, `LI`, `LK`, `LR`, `LS`, `LT`, `LU`, `LV`, `LY`, `MA`, `MC`, `MD`, `ME`, `MF`, `MG`, `MH`, `MK`, `ML`, `MM`, `MN`, `MO`, `MP`, `MQ`, `MR`, `MS`, `MT`, `MU`, `MV`, `MW`, `MX`, `MY`, `MZ`, `NA`, `NC`, `NE`, `NF`, `NG`, `NI`, `NL`, `NO`, `NP`, `NR`, `NU`, `NZ`, `OM`, `PA`, `PE`, `PF`, `PG`, `PH`, `PK`, `PL`, `PM`, `PN` |
| `nexusCountry.refName` | Reference Name | string |  |  |  |  |
| `nexusState` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `taxRegistrationNumber` | Tax Reg. Number | string |  |  |  |  |

## customerCollection

Browser definition `customerCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | customer[] |  |  | [`customer`](#customer) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customerSelectOptions

Browser definition `customerSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accessRole` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `alcoholRecipientType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `assignedWebSite` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingRateCard` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingTransactionForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingTransactionType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `buyingReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `buyingTimeFrame` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `campaignCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `campaignEvent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `category` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contact` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contactList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `creditHoldOverride` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultAllocationStrategy` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultBankAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultShippingAddress` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultTaxReg` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `drAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `emailPreference` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entityStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `fxAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `globalSubscriptionStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `image` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `language` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `leadSource` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `monthlyClosing` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `negativeNumberFormat` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `numberFormat` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `openingBalanceAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `partner` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `prefCcProcessor` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `priceLevel` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `receivablesAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `representingSubsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesReadiness` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesRep` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shippingCarrier` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shippingItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `sourceWebSite` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `symbolPlacement` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `terms` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `territory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `thirdPartyCarrier` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `thirdPartyCountry` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `topLevelParent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

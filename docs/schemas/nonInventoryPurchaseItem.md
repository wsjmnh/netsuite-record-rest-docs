# Schemas: nonInventoryPurchaseItem

Property tables for definitions owned by `nonInventoryPurchaseItem`.

Record page: [nonInventoryPurchaseItem](../records/nonInventoryPurchaseItem.md).

## Index

- [nonInventoryPurchaseItem](#noninventorypurchaseitem) — 81 properties
- [nonInventoryPurchaseItem-accountingBookDetailCollection](#noninventorypurchaseitem-accountingbookdetailcollection) — 6 properties
- [nonInventoryPurchaseItem-accountingBookDetailElement](#noninventorypurchaseitem-accountingbookdetailelement) — 11 properties
- [nonInventoryPurchaseItem-hierarchyVersionsCollection](#noninventorypurchaseitem-hierarchyversionscollection) — 6 properties
- [nonInventoryPurchaseItem-hierarchyVersionsElement](#noninventorypurchaseitem-hierarchyversionselement) — 7 properties
- [nonInventoryPurchaseItem-itemVendor-itemVendorPrice](#noninventorypurchaseitem-itemvendor-itemvendorprice) — 4 properties
- [nonInventoryPurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection](#noninventorypurchaseitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) — 6 properties
- [nonInventoryPurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement](#noninventorypurchaseitem-itemvendor-itemvendorprice-itemvendorpricelineselement) — 6 properties
- [nonInventoryPurchaseItem-itemVendorCollection](#noninventorypurchaseitem-itemvendorcollection) — 6 properties
- [nonInventoryPurchaseItem-itemVendorElement](#noninventorypurchaseitem-itemvendorelement) — 13 properties
- [nonInventoryPurchaseItem-translationsCollection](#noninventorypurchaseitem-translationscollection) — 6 properties
- [nonInventoryPurchaseItem-translationsElement](#noninventorypurchaseitem-translationselement) — 16 properties
- [nonInventoryPurchaseItemCollection](#noninventorypurchaseitemcollection) — 6 properties
- [nonInventoryPurchaseItemSelectOptions](#noninventorypurchaseitemselectoptions) — 32 properties

## nonInventoryPurchaseItem

Browser definition `nonInventoryPurchaseItem`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `VSOEDeferral` |  | object |  |  |  |  |
| `VSOEDeferral.id` | Internal identifier | string |  |  |  | `DEFERALLUNTIL`, `DEFERUNTIL` |
| `VSOEDeferral.refName` | Reference Name | string |  |  |  |  |
| `VSOEDelivered` | Default as Delivered | boolean |  |  |  |  |
| `VSOEPermitDiscount` |  | object |  |  |  |  |
| `VSOEPermitDiscount.id` | Internal identifier | string |  |  |  | `IFDELIVERED`, `NEVER` |
| `VSOEPermitDiscount.refName` | Reference Name | string |  |  |  |  |
| `VSOEPrice` | Allocation Price | number | double |  |  |  |
| `VSOESopGroup` |  | object |  |  |  |  |
| `VSOESopGroup.id` | Internal identifier | string |  |  |  | `EXCLUDE`, `NORMAL`, `SOFTWARE` |
| `VSOESopGroup.refName` | Reference Name | string |  |  |  |  |
| `accountingBookDetail` |  | nonInventoryPurchaseItem-accountingBookDetailCollection |  |  | [`nonInventoryPurchaseItem-accountingBookDetailCollection`](#noninventorypurchaseitem-accountingbookdetailcollection) |  |
| `amortizationPeriod` | Amortization Period | integer | int64 |  |  |  |
| `amortizationTemplate` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `availableToPartners` | Available to Adv. Partners | boolean |  |  |  |  |
| `baseUnit` | Primary Base Unit | string |  |  |  |  |
| `billExchRateVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `billPriceVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `billQtyVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `consumptionUnit` | Primary Consumption Unit | string |  |  |  |  |
| `cost` | Purchase Price | number | double |  |  |  |
| `costCategory` |  | costCategory |  |  | [`costCategory`](costCategory.md#costcategory) |  |
| `createExpensePlansOn` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deferralAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `displayName` | Display Name/Code | string |  |  |  |  |
| `exchangeRate` | Exchange Rate | string |  |  |  |  |
| `expenseAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `expenseAmortizationRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `generateAccruals` | Generate Accruals | boolean |  |  |  |  |
| `hierarchyVersions` |  | nonInventoryPurchaseItem-hierarchyVersionsCollection |  |  | [`nonInventoryPurchaseItem-hierarchyVersionsCollection`](#noninventorypurchaseitem-hierarchyversionscollection) |  |
| `id` | Internal ID | string |  |  |  |  |
| `includeChildren` | Include Children | boolean |  |  |  |  |
| `insertItemAttribute` |  | object |  |  |  |  |
| `insertItemAttribute.id` | Internal identifier | string |  |  |  | `class`, `department`, `location`, `itemid`, `issueproduct`, `vendorname` |
| `insertItemAttribute.refName` | Reference Name | string |  |  |  |  |
| `isFulfillable` | Can be Fulfilled | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isTaxable` | Taxable | boolean |  |  |  |  |
| `issueProduct` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `itemId` | Item Name/Number | string |  |  |  |  |
| `itemOptions` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `itemType` |  | object |  |  |  |  |
| `itemType.id` | Internal identifier | string |  |  |  | `Group`, `Description`, `Discount`, `EndGroup`, `GiftCert`, `Subtotal`, `Service`, `ShipItem`, `TaxItem`, `InvtPart`, `Payment`, `Expense`, `NonInvtPart`, `TaxGroup`, `Kit`, `Markup`, `DwnLdItem`, `OthCharge`, `Assembly`, `SubscriPlan` |
| `itemType.refName` | Reference Name | string |  |  |  |  |
| `itemVendor` |  | nonInventoryPurchaseItem-itemVendorCollection |  |  | [`nonInventoryPurchaseItem-itemVendorCollection`](#noninventorypurchaseitem-itemvendorcollection) |  |
| `lastModifiedDate` | Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `matrixItemNameTemplate` | Matrix Item Name Template | string |  |  |  |  |
| `matrixItemNameTemplateHelp` | Matrix Item Name Template | string |  |  |  |  |
| `matrixType` |  | object |  |  |  |  |
| `matrixType.id` | Internal identifier | string |  |  |  | `PARENT`, `CHILD` |
| `matrixType.refName` | Reference Name | string |  |  |  |  |
| `parent` |  | nonInventoryPurchaseItem |  |  | [`nonInventoryPurchaseItem`](#noninventorypurchaseitem) |  |
| `parentOnly` | Use as Category Only | boolean |  |  |  |  |
| `purchaseDescription` | Purchase Description | string |  |  |  |  |
| `purchaseOrderAmount` | Vendor Bill - Purchase Order Amount Tolerance | number | float |  |  |  |
| `purchaseOrderQuantity` | Vendor Bill - Purchase Order Quantity Tolerance | number | float |  |  |  |
| `purchaseOrderQuantityDiff` | Vendor Bill - Purchase Order Quantity Difference | number | float |  |  |  |
| `purchaseTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `purchaseUnit` | Primary Purchase Unit | string |  |  |  |  |
| `receiptAmount` | Vendor Bill - Item Receipt Amount Tolerance | number | float |  |  |  |
| `receiptQuantity` | Vendor Bill - Item Receipt Quantity Tolerance | number | float |  |  |  |
| `receiptQuantityDiff` | Vendor Bill - Item Receipt Quantity Difference | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `residual` | Residual | number | double |  |  |  |
| `salesTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `subsidiary` |  | subsidiaryCollection |  |  | [`subsidiaryCollection`](subsidiary.md#subsidiarycollection) |  |
| `taxSchedule` |  | taxSchedule |  |  | [`taxSchedule`](taxSchedule.md#taxschedule) |  |
| `translations` |  | nonInventoryPurchaseItem-translationsCollection |  |  | [`nonInventoryPurchaseItem-translationsCollection`](#noninventorypurchaseitem-translationscollection) |  |
| `unitsType` |  | unitsType |  |  | [`unitsType`](unitsType.md#unitstype) |  |
| `upcCode` | UPC Code | string |  |  |  |  |
| `vendor` |  | vendor |  |  | [`vendor`](vendor.md#vendor) |  |
| `vendorName` | Vendor Name/Code | string |  |  |  |  |

## nonInventoryPurchaseItem-accountingBookDetailCollection

Browser definition `nonInventoryPurchaseItem-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | nonInventoryPurchaseItem-accountingBookDetailElement[] |  |  | [`nonInventoryPurchaseItem-accountingBookDetailElement`](#noninventorypurchaseitem-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nonInventoryPurchaseItem-accountingBookDetailElement

Browser definition `nonInventoryPurchaseItem-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `amortizationTemplate` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `createExpensePlansOn` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `createRevenuePlansOn` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecForecastRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `revRecSchedule` |  | revRecTemplate |  |  | [`revRecTemplate`](revRecTemplate.md#revrectemplate) |  |
| `revenueRecognitionRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `sameAsPrimaryAmortization` | Same as Primary Book Amortization | boolean |  |  |  |  |
| `sameAsPrimaryRevRec` | Same as Primary Book Rev Rec | boolean |  |  |  |  |

## nonInventoryPurchaseItem-hierarchyVersionsCollection

Browser definition `nonInventoryPurchaseItem-hierarchyVersionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | nonInventoryPurchaseItem-hierarchyVersionsElement[] |  |  | [`nonInventoryPurchaseItem-hierarchyVersionsElement`](#noninventorypurchaseitem-hierarchyversionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nonInventoryPurchaseItem-hierarchyVersionsElement

Browser definition `nonInventoryPurchaseItem-hierarchyVersionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `endDate` | Hierarchy Version End Date | string | date |  |  |  |
| `hierarchyNode` |  | merchandiseHierarchyNode |  |  | [`merchandiseHierarchyNode`](merchandiseHierarchyNode.md#merchandisehierarchynode) |  |
| `hierarchyVersion` |  | merchandiseHierarchyVersion |  |  | [`merchandiseHierarchyVersion`](merchandiseHierarchyVersion.md#merchandisehierarchyversion) |  |
| `isIncluded` | Included In Version | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `startDate` | Hierarchy Version Start Date | string | date |  |  |  |

## nonInventoryPurchaseItem-itemVendor-itemVendorPrice

Browser definition `nonInventoryPurchaseItem-itemVendor-itemVendorPrice`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `externalId` | External ID | string |  |  |  |  |
| `itemvendorpricelines` |  | nonInventoryPurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection |  |  | [`nonInventoryPurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](#noninventorypurchaseitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## nonInventoryPurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection

Browser definition `nonInventoryPurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | nonInventoryPurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement[] |  |  | [`nonInventoryPurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](#noninventorypurchaseitem-itemvendor-itemvendorprice-itemvendorpricelineselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nonInventoryPurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement

Browser definition `nonInventoryPurchaseItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `vendorCost` | Vendor Cost | number | double |  |  |  |
| `vendorcurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `vendorprice` | Purchase Price | number | double |  |  |  |

## nonInventoryPurchaseItem-itemVendorCollection

Browser definition `nonInventoryPurchaseItem-itemVendorCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | nonInventoryPurchaseItem-itemVendorElement[] |  |  | [`nonInventoryPurchaseItem-itemVendorElement`](#noninventorypurchaseitem-itemvendorelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nonInventoryPurchaseItem-itemVendorElement

Browser definition `nonInventoryPurchaseItem-itemVendorElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `itemVendorPrice` |  | nonInventoryPurchaseItem-itemVendor-itemVendorPrice |  |  | [`nonInventoryPurchaseItem-itemVendor-itemVendorPrice`](#noninventorypurchaseitem-itemvendor-itemvendorprice) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `predConfidence` | Predicted Risk Confidence | number | double |  |  |  |
| `predictedDays` | Predicted Days Late/Early | integer | int64 |  |  |  |
| `preferredVendor` | Preferred | boolean |  |  |  |  |
| `purchasePrice` | Purchase Price | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `schedule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `vendor` |  | vendor |  |  | [`vendor`](vendor.md#vendor) |  |
| `vendorCode` | Code | string |  |  |  |  |
| `vendorCurrencyId` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `vendorCurrencyName` | Currency | string |  |  |  |  |

## nonInventoryPurchaseItem-translationsCollection

Browser definition `nonInventoryPurchaseItem-translationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | nonInventoryPurchaseItem-translationsElement[] |  |  | [`nonInventoryPurchaseItem-translationsElement`](#noninventorypurchaseitem-translationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nonInventoryPurchaseItem-translationsElement

Browser definition `nonInventoryPurchaseItem-translationsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `displayName` | Display Name | string |  |  |  |  |
| `featuredDescription` | Featured Description | string |  |  |  |  |
| `language` | Language | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `locale` |  | object |  |  |  |  |
| `locale.id` | Internal identifier | string |  |  |  | `it_CH`, `en_TC`, `af_ZA`, `es_EA`, `es_EC`, `pt_BR`, `en_CY`, `fr_LU`, `nl_AN`, `es_UY`, `en_TT`, `es_ES`, `pt_ST`, `en_DM`, `en_TZ`, `es_ES_EURO`, `fr_ML`, `de_DE_onLQA`, `es_VE`, `nl_BE`, `da_DK`, `pt_AO`, `to_TO`, `en_UG`, `am_ET`, `ss_SZ`, `nl_BQ`, `ar`, `pt_AW`, `ko_KR`, `en_US`, `fr_BE_EURO`, `ko_KP`, `si_AQ`, `fr_MG`, `el_GR`, `be_BY`, `en_AU`, `he_IL`, `en_AW`, `es_SV`, `en_BB`, `ar_YE`, `es_CO`, `es_CL`, `en_BM`, `es_CR`, `pa_IN`, `en_SC`, `en_BS`, `sm_WS`, `it_IT_EURO`, `fr_KM`, `es_CU`, `en_SB`, `en_SG`, `en_BW`, `en_SH`, `en_BZ`, `en_SL`, `az_AZ`, `fi_FI`, `en_SS`, `sr_YU`, `en_CD`, `en_CA`, `ka_GE`, `lv_LV`, `uk_UA`, `es_DO`, `ur_PK`, `ar_IQ`, `fr_LU_EURO`, `pt_PT`, `fr_FR_EURO`, `en_PH`, `th_TH`, `bn_BD`, `si_LK`, `en_PG`, `hu_HU`, `ar_SA`, `ar_SD`, `ru_KZ`, `ar_BH`, `nl_BE_EURO`, `ro_MD`, `en_QA`, `ru_KG`, `es_AR`, `ta_IN`, `sr_RS`, `aa_ER`, `en`, `de_DE_EURO`, `zh_MO`, `en_AE`, `ar_SY`, `es_BO`, `en_AI`, `no_NO`, `en_AG`, `nl_SR`, `fr_VU`, `en_MW`, `gu_AQ`, `ar_TN`, `nl_SX`, `hi_IN`, `en_NA`, `mn_MN`, `en_NG`, `fr_FR`, `ms_MY`, `nl_CW`, `uz_UZ`, `ar_DJ`, `sr_CS`, `de_AT_EURO`, `en_NZ`, `es_PE`, `es_PA`, `fa_IR`, `ar_DZ`, `fr_GN`, `lb_LU`, `xx_US`, `pt_CV`, `sh_RS`, `ht_HT`, `fr_WF`, `es_AR_onLQA`, `es_PR`, `ar_EG`, `es_PY`, `fr_GA`, `en_KW`, `de_AT`, `ro_RO`, `en_KY`, `fr_FR_onLQA`, `fr_DJ`, `ca_ES_EURO`, `cs_CZ`, `en_LC`, `pl_AQ`, `fr_TD`, `fr_TG`, `es_MX`, `sv_AX`, `sk_SK`, `en_LR`, `en_LS`, `ar_OM`, `dz_BT`, `te_IN`, `de_LU_EURO`, `sq_AL`, `sv_SE`, `sn_ZW`, `es_NI`, `en_IE_EURO`, `my_MM`, `en_MF`, `en_MU`, `it_IT`, `pl_PL`, `fr_BE`, `fr_BF`, `tr_TR`, `fr_BI`, `fr_BJ`, `id_ID`, `fr_RW`, `en_ZM`, `km_KH`, `ja_JP`, `de_DE`, `fr_BL`, `tg_TJ`, `ar_QA`, `de_CH`, `zh_HK`, `pt_PT_EURO`, `en_JO`, `en_JM`, `fr_CA`, `nl_NL_EURO`, `fr_CF`, `fr_CG`, `fr_CD`, `pa_AQ`, `fr_CH`, `xx_US_wthId`, `fr_CI`, `pt_GW`, `vi_VN`, `ru_MD`, `fr_CM`, `fr_SC`, `en_KE`, `ne_NP`, `bs_BA`, `sl_SI`, `en_KN`, `fr_SN`, `ar_AE`, `en_GY`, `tl_PH`, `ca_ES`, `es_IC`, `lo_LA`, `kn_IN`, `so_SO`, `fr_PF`, `ar_JO`, `nl_NL`, `is_IS`, `fi_FI_EURO`, `pt_MZ`, `sk_SK_EURO`, `sl_SI_EURO`, `en_IE`, `ms_BN`, `hr_HR`, `ar_KW`, `de_LU`, `lt_LT`, `en_IN`, `ps_AF`, `en_ZA`, `en_VC`, `ru_RU`, `sh_YU`, `ar_LB`, `mr_IN`, `dv_MV`, `fj_FJ`, `zh_TW`, `tk_TM`, `ar_LY`, `en_VU`, `fr_NE`, `en_FK`, `es_GT`, `fr_NC`, `es_GQ`, `fa_AF`, `bg_BG`, `hy_AM`, `en_CY_EURO`, `mk_MK`, `ar_MA`, `en_GD`, `en_GB`, `es_HN`, `gu_IN`, `en_GH`, `et_EE`, `en_GI`, `zh_CN`, `en_GM`, `ar_MR` |
| `locale.refName` | Reference Name | string |  |  |  |  |
| `noPriceMessage` | No Price Message | string |  |  |  |  |
| `outOfStockMessage` | Out Of Stock Message | string |  |  |  |  |
| `pageTitle` | Page Title | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `salesDescription` | Sales Description | string |  |  |  |  |
| `specialsDescription` | Special Description | string |  |  |  |  |
| `storeDescription` | Store Description | string |  |  |  |  |
| `storeDetailedDescription` | Detailed Description | string |  |  |  |  |
| `storeDisplayName` | Store Display Name | string |  |  |  |  |

## nonInventoryPurchaseItemCollection

Browser definition `nonInventoryPurchaseItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | nonInventoryPurchaseItem[] |  |  | [`nonInventoryPurchaseItem`](#noninventorypurchaseitem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nonInventoryPurchaseItemSelectOptions

Browser definition `nonInventoryPurchaseItemSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `VSOEDeferral` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `VSOEPermitDiscount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `VSOESopGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `amortizationTemplate` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `baseUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billExchRateVarianceAcct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billPriceVarianceAcct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billQtyVarianceAcct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `consumptionUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `costCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createExpensePlansOn` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deferralAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `expenseAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `expenseAmortizationRule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `insertItemAttribute` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `issueProduct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemOptions` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `matrixType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `purchaseTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `purchaseUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `unitsType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `vendor` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

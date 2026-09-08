# Schemas: otherChargeSaleItem

Property tables for definitions owned by `otherChargeSaleItem`.

Record page: [otherChargeSaleItem](../records/otherChargeSaleItem.md).

## Index

- [otherChargeSaleItem](#otherchargesaleitem) — 105 properties
- [otherChargeSaleItem-accountingBookDetailCollection](#otherchargesaleitem-accountingbookdetailcollection) — 6 properties
- [otherChargeSaleItem-accountingBookDetailElement](#otherchargesaleitem-accountingbookdetailelement) — 11 properties
- [otherChargeSaleItem-hierarchyVersionsCollection](#otherchargesaleitem-hierarchyversionscollection) — 6 properties
- [otherChargeSaleItem-hierarchyVersionsElement](#otherchargesaleitem-hierarchyversionselement) — 7 properties
- [otherChargeSaleItem-price](#otherchargesaleitem-price) — 6 properties
- [otherChargeSaleItem-priceElement](#otherchargesaleitem-priceelement) — 10 properties
- [otherChargeSaleItem-translationsCollection](#otherchargesaleitem-translationscollection) — 6 properties
- [otherChargeSaleItem-translationsElement](#otherchargesaleitem-translationselement) — 16 properties
- [otherChargeSaleItemCollection](#otherchargesaleitemcollection) — 6 properties
- [otherChargeSaleItemSelectOptions](#otherchargesaleitemselectoptions) — 43 properties

## otherChargeSaleItem

Browser definition `otherChargeSaleItem`.

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
| `accountingBookDetail` |  | otherChargeSaleItem-accountingBookDetailCollection |  |  | [`otherChargeSaleItem-accountingBookDetailCollection`](#otherchargesaleitem-accountingbookdetailcollection) |  |
| `amortizationPeriod` | Amortization Period | integer | int64 |  |  |  |
| `amortizationTemplate` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `autoExpandKitForRevenuemgmt` | Auto-Expansion for Revenue Management | boolean |  |  |  |  |
| `availableToPartners` | Available to Adv. Partners | boolean |  |  |  |  |
| `baseUnit` | Primary Base Unit | string |  |  |  |  |
| `billExchRateVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `billPriceVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `billQtyVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `billingSchedule` |  | billingSchedule |  |  | [`billingSchedule`](billingSchedule.md#billingschedule) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `consumptionUnit` | Primary Consumption Unit | string |  |  |  |  |
| `contingentRevenueHandling` | Eligible For Contingent Revenue Handling | boolean |  |  |  |  |
| `costCategory` |  | costCategory |  |  | [`costCategory`](costCategory.md#costcategory) |  |
| `costEstimate` | Item Defined Cost | number | double |  |  |  |
| `costEstimateUnits` | Est. Cost Unit | string |  |  |  |  |
| `costForPricing` | Cost for Pricing | number | double |  |  |  |
| `createExpensePlansOn` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `createRevenuePlansOn` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deferRevRec` | Hold Revenue Recognition | boolean |  |  |  |  |
| `deferralAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `deferredRevenueAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `directRevenuePosting` | Direct Revenue Posting | boolean |  |  |  |  |
| `displayName` | Display Name/Code | string |  |  |  |  |
| `enforceminqtyinternally` | Enforce Minimum Internally | boolean |  |  |  |  |
| `expenseAmortizationRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `hierarchyVersions` |  | otherChargeSaleItem-hierarchyVersionsCollection |  |  | [`otherChargeSaleItem-hierarchyVersionsCollection`](#otherchargesaleitem-hierarchyversionscollection) |  |
| `id` | Internal ID | string |  |  |  |  |
| `includeChildren` | Include Children | boolean |  |  |  |  |
| `incomeAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `insertItemAttribute` |  | object |  |  |  |  |
| `insertItemAttribute.id` | Internal identifier | string |  |  |  | `class`, `department`, `location`, `itemid`, `issueproduct`, `vendorname` |
| `insertItemAttribute.refName` | Reference Name | string |  |  |  |  |
| `isFulfillable` | Can be Fulfilled | boolean |  |  |  |  |
| `isGCoCompliant` | Google Checkout Compliant | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isOnline` | Display in Website | boolean |  |  |  |  |
| `isTaxable` | Taxable | boolean |  |  |  |  |
| `issueProduct` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `itemId` | Item Name/Number | string |  |  |  |  |
| `itemOptions` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `itemRevenueCategory` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `itemType` |  | object |  |  |  |  |
| `itemType.id` | Internal identifier | string |  |  |  | `Group`, `Description`, `Discount`, `EndGroup`, `GiftCert`, `Subtotal`, `Service`, `ShipItem`, `TaxItem`, `InvtPart`, `Payment`, `Expense`, `NonInvtPart`, `TaxGroup`, `Kit`, `Markup`, `DwnLdItem`, `OthCharge`, `Assembly`, `SubscriPlan` |
| `itemType.refName` | Reference Name | string |  |  |  |  |
| `lastModifiedDate` | Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `matrixItemNameTemplate` | Matrix Item Name Template | string |  |  |  |  |
| `matrixItemNameTemplateHelp` | Matrix Item Name Template | string |  |  |  |  |
| `matrixType` |  | object |  |  |  |  |
| `matrixType.id` | Internal identifier | string |  |  |  | `PARENT`, `CHILD` |
| `matrixType.refName` | Reference Name | string |  |  |  |  |
| `maximumquantity` | Maximum Order Qty | integer | int64 |  |  |  |
| `minimumquantity` | Minimum Order Qty | integer | int64 |  |  |  |
| `offerSupport` | Offer Support | boolean |  |  |  |  |
| `overallQuantityPricingType` |  | object |  |  |  |  |
| `overallQuantityPricingType.id` | Internal identifier | string |  |  |  | `ITEM`, `PARENT`, `SCHEDULE` |
| `overallQuantityPricingType.refName` | Reference Name | string |  |  |  |  |
| `parent` |  | otherChargeSaleItem |  |  | [`otherChargeSaleItem`](#otherchargesaleitem) |  |
| `parentOnly` | Use as Category Only | boolean |  |  |  |  |
| `price` |  | otherChargeSaleItem-price |  |  | [`otherChargeSaleItem-price`](#otherchargesaleitem-price) |  |
| `pricesIncludeTax` | Prices Include Tax | boolean |  |  |  |  |
| `pricingGroup` |  | pricingGroup |  |  | [`pricingGroup`](pricingGroup.md#pricinggroup) |  |
| `quantityPricingSchedule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `rate` | Price | number | double |  |  |  |
| `rateIncludingTax` | Price Including Tax | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `residual` | Residual | number | double |  |  |  |
| `revRecForecastRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `revRecSchedule` |  | revRecTemplate |  |  | [`revRecTemplate`](revRecTemplate.md#revrectemplate) |  |
| `revReclassFxAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `revenueAllocationGroup` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `revenueRecognitionRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `saleUnit` | Primary Sale Unit | string |  |  |  |  |
| `salesDescription` | Sales Description | string |  |  |  |  |
| `salesTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `softDescriptor` |  | object |  |  |  |  |
| `softDescriptor.id` | Internal identifier | string |  |  |  | `1`, `2` |
| `softDescriptor.refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiaryCollection |  |  | [`subsidiaryCollection`](subsidiary.md#subsidiarycollection) |  |
| `subtype` |  | object |  |  |  |  |
| `subtype.id` | Internal identifier | string |  |  |  | `Sale`, `Purchase`, `Resale` |
| `subtype.refName` | Reference Name | string |  |  |  |  |
| `taxSchedule` |  | taxSchedule |  |  | [`taxSchedule`](taxSchedule.md#taxschedule) |  |
| `translations` |  | otherChargeSaleItem-translationsCollection |  |  | [`otherChargeSaleItem-translationsCollection`](#otherchargesaleitem-translationscollection) |  |
| `unitsType` |  | unitsType |  |  | [`unitsType`](unitsType.md#unitstype) |  |
| `upcCode` | UPC Code | string |  |  |  |  |
| `useMarginalRates` | Use Marginal Rates | boolean |  |  |  |  |

## otherChargeSaleItem-accountingBookDetailCollection

Browser definition `otherChargeSaleItem-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | otherChargeSaleItem-accountingBookDetailElement[] |  |  | [`otherChargeSaleItem-accountingBookDetailElement`](#otherchargesaleitem-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## otherChargeSaleItem-accountingBookDetailElement

Browser definition `otherChargeSaleItem-accountingBookDetailElement`.

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

## otherChargeSaleItem-hierarchyVersionsCollection

Browser definition `otherChargeSaleItem-hierarchyVersionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | otherChargeSaleItem-hierarchyVersionsElement[] |  |  | [`otherChargeSaleItem-hierarchyVersionsElement`](#otherchargesaleitem-hierarchyversionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## otherChargeSaleItem-hierarchyVersionsElement

Browser definition `otherChargeSaleItem-hierarchyVersionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `endDate` | Hierarchy Version End Date | string | date |  |  |  |
| `hierarchyNode` |  | merchandiseHierarchyNode |  |  | [`merchandiseHierarchyNode`](merchandiseHierarchyNode.md#merchandisehierarchynode) |  |
| `hierarchyVersion` |  | merchandiseHierarchyVersion |  |  | [`merchandiseHierarchyVersion`](merchandiseHierarchyVersion.md#merchandisehierarchyversion) |  |
| `isIncluded` | Included In Version | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `startDate` | Hierarchy Version Start Date | string | date |  |  |  |

## otherChargeSaleItem-price

Browser definition `otherChargeSaleItem-price`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | otherChargeSaleItem-priceElement[] |  |  | [`otherChargeSaleItem-priceElement`](#otherchargesaleitem-priceelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## otherChargeSaleItem-priceElement

Browser definition `otherChargeSaleItem-priceElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `currencyPage` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `discountDisplay` | Default Discount % | number | double |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `price` | Amount | number | double |  |  |  |
| `priceLevel` |  | priceLevel |  |  | [`priceLevel`](priceLevel.md#pricelevel) |  |
| `priceLevelName` | Price Level | string |  |  |  |  |
| `priceQty` | Sequence Number | integer | int64 |  |  |  |
| `quantity` |  | array |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## otherChargeSaleItem-translationsCollection

Browser definition `otherChargeSaleItem-translationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | otherChargeSaleItem-translationsElement[] |  |  | [`otherChargeSaleItem-translationsElement`](#otherchargesaleitem-translationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## otherChargeSaleItem-translationsElement

Browser definition `otherChargeSaleItem-translationsElement`.

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

## otherChargeSaleItemCollection

Browser definition `otherChargeSaleItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | otherChargeSaleItem[] |  |  | [`otherChargeSaleItem`](#otherchargesaleitem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## otherChargeSaleItemSelectOptions

Browser definition `otherChargeSaleItemSelectOptions`.

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
| `billingSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `consumptionUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `costCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createExpensePlansOn` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createRevenuePlansOn` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deferralAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deferredRevenueAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `expenseAmortizationRule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `incomeAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `insertItemAttribute` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `issueProduct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemOptions` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemRevenueCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `matrixType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `overallQuantityPricingType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `pricingGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `quantityPricingSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revRecForecastRule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revRecSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revReclassFxAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revenueAllocationGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revenueRecognitionRule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `saleUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `softDescriptor` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subtype` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `unitsType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

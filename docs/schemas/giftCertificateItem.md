# Schemas: giftCertificateItem

Property tables for definitions owned by `giftCertificateItem`.

Record page: [giftCertificateItem](../records/giftCertificateItem.md).

## Index

- [giftCertificateItem](#giftcertificateitem) — 81 properties
- [giftCertificateItem-authCodesCollection](#giftcertificateitem-authcodescollection) — 6 properties
- [giftCertificateItem-authCodesElement](#giftcertificateitem-authcodeselement) — 4 properties
- [giftCertificateItem-correlatedItemsCollection](#giftcertificateitem-correlateditemscollection) — 6 properties
- [giftCertificateItem-correlatedItemsElement](#giftcertificateitem-correlateditemselement) — 7 properties
- [giftCertificateItem-presentationItemCollection](#giftcertificateitem-presentationitemcollection) — 6 properties
- [giftCertificateItem-presentationItemElement](#giftcertificateitem-presentationitemelement) — 11 properties
- [giftCertificateItem-price](#giftcertificateitem-price) — 6 properties
- [giftCertificateItem-priceElement](#giftcertificateitem-priceelement) — 6 properties
- [giftCertificateItem-siteCategoryCollection](#giftcertificateitem-sitecategorycollection) — 6 properties
- [giftCertificateItem-siteCategoryElement](#giftcertificateitem-sitecategoryelement) — 4 properties
- [giftCertificateItem-translationsCollection](#giftcertificateitem-translationscollection) — 6 properties
- [giftCertificateItem-translationsElement](#giftcertificateitem-translationselement) — 16 properties
- [giftCertificateItemCollection](#giftcertificateitemcollection) — 6 properties
- [giftCertificateItemSelectOptions](#giftcertificateitemselectoptions) — 21 properties

## giftCertificateItem

Browser definition `giftCertificateItem`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `authCodes` |  | giftCertificateItem-authCodesCollection |  |  | [`giftCertificateItem-authCodesCollection`](#giftcertificateitem-authcodescollection) |  |
| `availableToPartners` | Available to Adv. Partners | boolean |  |  |  |  |
| `billingSchedule` |  | billingSchedule |  |  | [`billingSchedule`](billingSchedule.md#billingschedule) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `correlatedItems` |  | giftCertificateItem-correlatedItemsCollection |  |  | [`giftCertificateItem-correlatedItemsCollection`](#giftcertificateitem-correlateditemscollection) |  |
| `costEstimate` | Item Defined Cost | number | double |  |  |  |
| `costForPricing` | Cost for Pricing | number | double |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `daysBeforeExpiration` | Days Before Expiration | integer | int64 |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `displayName` | Display Name/Code | string |  |  |  |  |
| `dontShowPrice` | Don't Show Price | boolean |  |  |  |  |
| `excludeFromSiteMap` | Exclude from Sitemap | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `featuredDescription` | Featured Description | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `includeChildren` | Include Children | boolean |  |  |  |  |
| `incomeAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `isDonationItem` | Variable Amount | boolean |  |  |  |  |
| `isFulfillable` | Can be Fulfilled | boolean |  |  |  |  |
| `isGCoCompliant` | Google Checkout Compliant | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isOnline` | Display in Website | boolean |  |  |  |  |
| `isTaxable` | Taxable | boolean |  |  |  |  |
| `issueProduct` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `itemId` | Item Name/Number | string |  |  |  |  |
| `itemOptions` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `itemType` |  | object |  |  |  |  |
| `itemType.id` | Internal identifier | string |  |  |  | `Group`, `Description`, `Discount`, `EndGroup`, `GiftCert`, `Subtotal`, `Service`, `ShipItem`, `TaxItem`, `InvtPart`, `Payment`, `Expense`, `NonInvtPart`, `TaxGroup`, `Kit`, `Markup`, `DwnLdItem`, `OthCharge`, `Assembly`, `SubscriPlan` |
| `itemType.refName` | Reference Name | string |  |  |  |  |
| `lastModifiedDate` | Last Modified | string | date-time |  |  |  |
| `liabilityAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `maxDonationAmount` | Maximum Variable Amount | number | double |  |  |  |
| `metaTagHtml` | Meta Tag HTML | string |  |  |  |  |
| `noPriceMessage` | No Price Message | string |  |  |  |  |
| `offerSupport` | Offer Support | boolean |  |  |  |  |
| `onSpecial` | On Special | boolean |  |  |  |  |
| `outOfStockBehavior` |  | object |  |  |  |  |
| `outOfStockBehavior.id` | Internal identifier | string |  |  |  | `DISABLE`, `ENABLENMSG`, `REMOVE`, `ENABLE`, `DEFAULT` |
| `outOfStockBehavior.refName` | Reference Name | string |  |  |  |  |
| `outOfStockMessage` | Out Of Stock Message | string |  |  |  |  |
| `pageTitle` | Page Title | string |  |  |  |  |
| `parent` |  | giftCertificateItem |  |  | [`giftCertificateItem`](#giftcertificateitem) |  |
| `parentOnly` | Use as Category Only | boolean |  |  |  |  |
| `presentationItem` |  | giftCertificateItem-presentationItemCollection |  |  | [`giftCertificateItem-presentationItemCollection`](#giftcertificateitem-presentationitemcollection) |  |
| `price` |  | giftCertificateItem-price |  |  | [`giftCertificateItem-price`](#giftcertificateitem-price) |  |
| `pricesIncludeTax` | Prices Include Tax | boolean |  |  |  |  |
| `pricingGroup` |  | pricingGroup |  |  | [`pricingGroup`](pricingGroup.md#pricinggroup) |  |
| `rate` | Price | number | double |  |  |  |
| `rateIncludingTax` | Price Including Tax | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `relatedItemsDescription` | Related Items Description | string |  |  |  |  |
| `salesDescription` | Sales Description | string |  |  |  |  |
| `salesTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `searchKeywords` | Search Keywords | string |  |  |  |  |
| `showDefaultDonationAmount` | Show Default Amount | boolean |  |  |  |  |
| `siteCategory` |  | giftCertificateItem-siteCategoryCollection |  |  | [`giftCertificateItem-siteCategoryCollection`](#giftcertificateitem-sitecategorycollection) |  |
| `siteMapPriority` |  | object |  |  |  |  |
| `siteMapPriority.id` | Internal identifier | string |  |  |  | `0.0`, `0.1`, `0.2`, `0.3`, `0.4`, `0.5`, `0.6`, `0.7`, `0.8`, `0.9`, `1.0` |
| `siteMapPriority.refName` | Reference Name | string |  |  |  |  |
| `storeDescription` | Store Description | string |  |  |  |  |
| `storeDetailedDescription` | Detailed Description | string |  |  |  |  |
| `storeDisplayImage` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `storeDisplayName` | Store Display Name | string |  |  |  |  |
| `storeDisplayThumbnail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `storeItemTemplate` |  | object |  |  |  |  |
| `storeItemTemplate.id` | Internal identifier | string |  |  |  | `-134`, `-178`, `-133`, `-177`, `-136`, `-179`, `-135`, `-130`, `-174`, `-173`, `-176`, `-132`, `-131`, `-175`, `-138`, `-137`, `-139`, `-150`, `-101`, `-145`, `-144`, `-100`, `-103`, `-147`, `-102`, `-146`, `-141`, `-140`, `-143`, `-142`, `-109`, `-108`, `-149`, `-105`, `-148`, `-104`, `-107`, `-106`, `-161`, `-160`, `-156`, `-112`, `-111`, `-155`, `-158`, `-114`, `-157`, `-113`, `-110`, `-154`, `-153`, `-119`, `-116`, `-159`, `-115`, `-118`, `-117`, `-170`, `-172`, `-171`, `-123`, `-122`, `-125`, `-124`, `-162`, `-121`, `-120`, `-127`, `-126`, `-129`, `-128` |
| `storeItemTemplate.refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiaryCollection |  |  | [`subsidiaryCollection`](subsidiary.md#subsidiarycollection) |  |
| `subtype` |  | object |  |  |  |  |
| `subtype.id` | Internal identifier | string |  |  |  | `Sale`, `Purchase`, `Resale` |
| `subtype.refName` | Reference Name | string |  |  |  |  |
| `taxSchedule` |  | taxSchedule |  |  | [`taxSchedule`](taxSchedule.md#taxschedule) |  |
| `translations` |  | giftCertificateItem-translationsCollection |  |  | [`giftCertificateItem-translationsCollection`](#giftcertificateitem-translationscollection) |  |
| `upcCode` | UPC Code | string |  |  |  |  |
| `urlComponent` | URL Component | string |  |  |  |  |

## giftCertificateItem-authCodesCollection

Browser definition `giftCertificateItem-authCodesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | giftCertificateItem-authCodesElement[] |  |  | [`giftCertificateItem-authCodesElement`](#giftcertificateitem-authcodeselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## giftCertificateItem-authCodesElement

Browser definition `giftCertificateItem-authCodesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `authCode` | Auth. Code | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `used` | Used | boolean |  |  |  |  |

## giftCertificateItem-correlatedItemsCollection

Browser definition `giftCertificateItem-correlatedItemsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | giftCertificateItem-correlatedItemsElement[] |  |  | [`giftCertificateItem-correlatedItemsElement`](#giftcertificateitem-correlateditemselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## giftCertificateItem-correlatedItemsElement

Browser definition `giftCertificateItem-correlatedItemsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `correlationFld` | Correlation % | number | double |  |  |  |
| `countFld` | Count | integer | int64 |  |  |  |
| `itemNKeyFld` | Item | string |  |  |  |  |
| `liftFld` | Lift % | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `purchaseRateFld` | Overall Purchase Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## giftCertificateItem-presentationItemCollection

Browser definition `giftCertificateItem-presentationItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | giftCertificateItem-presentationItemElement[] |  |  | [`giftCertificateItem-presentationItemElement`](#giftcertificateitem-presentationitemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## giftCertificateItem-presentationItemElement

Browser definition `giftCertificateItem-presentationItemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `basePrice` | Base Price | number | double |  |  |  |
| `description` | Item Description | string |  |  |  |  |
| `item` | Item | integer | int64 |  |  |  |
| `itemType` |  | object |  |  |  |  |
| `itemType.id` | Internal identifier | string |  |  |  | `FILECABITEM`, `PRESCATEGORY`, `INVTITEM`, `INFOITEM` |
| `itemType.refName` | Reference Name | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `onlinePrice` | Online Price | number | double |  |  |  |
| `presItemId` | Internal ID | integer | int64 |  |  |  |
| `presitemurl` | Item URL | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## giftCertificateItem-price

Browser definition `giftCertificateItem-price`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | giftCertificateItem-priceElement[] |  |  | [`giftCertificateItem-priceElement`](#giftcertificateitem-priceelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## giftCertificateItem-priceElement

Browser definition `giftCertificateItem-priceElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `price` | Amount | number | double |  |  |  |
| `priceLevel` |  | priceLevel |  |  | [`priceLevel`](priceLevel.md#pricelevel) |  |
| `priceQty` | Sequence Number | integer | int64 |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## giftCertificateItem-siteCategoryCollection

Browser definition `giftCertificateItem-siteCategoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | giftCertificateItem-siteCategoryElement[] |  |  | [`giftCertificateItem-siteCategoryElement`](#giftcertificateitem-sitecategoryelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## giftCertificateItem-siteCategoryElement

Browser definition `giftCertificateItem-siteCategoryElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `category` |  | siteCategory |  |  | [`siteCategory`](siteCategory.md#sitecategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `webSite` |  | webSite |  |  | [`webSite`](webSite.md#website) |  |

## giftCertificateItem-translationsCollection

Browser definition `giftCertificateItem-translationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | giftCertificateItem-translationsElement[] |  |  | [`giftCertificateItem-translationsElement`](#giftcertificateitem-translationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## giftCertificateItem-translationsElement

Browser definition `giftCertificateItem-translationsElement`.

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

## giftCertificateItemCollection

Browser definition `giftCertificateItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | giftCertificateItem[] |  |  | [`giftCertificateItem`](#giftcertificateitem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## giftCertificateItemSelectOptions

Browser definition `giftCertificateItemSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billingSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `incomeAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `issueProduct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemOptions` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `liabilityAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `outOfStockBehavior` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `pricingGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `siteMapPriority` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `storeDisplayImage` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `storeDisplayThumbnail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `storeItemTemplate` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subtype` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

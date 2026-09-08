# Schemas: siteCategory

Property tables for definitions owned by `siteCategory`.

Record page: [siteCategory](../records/siteCategory.md).

## Index

- [siteCategory](#sitecategory) — 35 properties
- [siteCategory-currentaudienceCollection](#sitecategory-currentaudiencecollection) — 6 properties
- [siteCategory-currentaudienceElement](#sitecategory-currentaudienceelement) — 3 properties
- [siteCategory-presentationItemCollection](#sitecategory-presentationitemcollection) — 6 properties
- [siteCategory-presentationItemElement](#sitecategory-presentationitemelement) — 15 properties
- [siteCategory-tag_subs_machineCollection](#sitecategory-tag_subs_machinecollection) — 6 properties
- [siteCategory-tag_subs_machineElement](#sitecategory-tag_subs_machineelement) — 4 properties
- [siteCategory-translationsCollection](#sitecategory-translationscollection) — 6 properties
- [siteCategory-translationsElement](#sitecategory-translationselement) — 10 properties
- [siteCategory-urlcomponentaliasesCollection](#sitecategory-urlcomponentaliasescollection) — 6 properties
- [siteCategory-urlcomponentaliasesElement](#sitecategory-urlcomponentaliaseselement) — 3 properties
- [siteCategoryCollection](#sitecategorycollection) — 6 properties
- [siteCategorySelectOptions](#sitecategoryselectoptions) — 10 properties

## siteCategory

Browser definition `siteCategory`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `categoryListLayout` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `correlatedItemsListLayout` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `currentaudience` |  | siteCategory-currentaudienceCollection |  |  | [`siteCategory-currentaudienceCollection`](#sitecategory-currentaudiencecollection) |  |
| `description` | Description | string |  |  |  |  |
| `excludeFromSiteMap` | Exclude from Sitemap | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fullName` | Full Name | string |  |  |  |  |
| `hierarchyRawFullName` | Full Name (Raw) | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isOnline` | Display in Website | boolean |  |  |  |  |
| `itemId` | Category | string |  |  |  |  |
| `itemListLayout` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `metaTagHtml` | Meta Tag HTML | string |  |  |  |  |
| `pageTitle` | Page Title | string |  |  |  |  |
| `parentCategory` |  | siteCategory |  |  | [`siteCategory`](#sitecategory) |  |
| `presentationItem` |  | siteCategory-presentationItemCollection |  |  | [`siteCategory-presentationItemCollection`](#sitecategory-presentationitemcollection) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `relatedItemsListLayout` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `searchKeywords` | Search Keywords | string |  |  |  |  |
| `siteCategoryType` |  | object |  |  |  |  |
| `siteCategoryType.id` | Internal identifier | string |  |  |  | `SS`, `PRES`, `CORREL`, `EL`, `KB`, `REL` |
| `siteCategoryType.refName` | Reference Name | string |  |  |  |  |
| `siteMapPriority` |  | object |  |  |  |  |
| `siteMapPriority.id` | Internal identifier | string |  |  |  | `0.0`, `0.1`, `0.2`, `0.3`, `0.4`, `0.5`, `0.6`, `0.7`, `0.8`, `0.9`, `1.0` |
| `siteMapPriority.refName` | Reference Name | string |  |  |  |  |
| `storeDetailedDescription` | Detailed Description | string |  |  |  |  |
| `storeDisplayImage` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `storeDisplayThumbnail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `tag_subs_machine` |  | siteCategory-tag_subs_machineCollection |  |  | [`siteCategory-tag_subs_machineCollection`](#sitecategory-tag_subs_machinecollection) |  |
| `translations` |  | siteCategory-translationsCollection |  |  | [`siteCategory-translationsCollection`](#sitecategory-translationscollection) |  |
| `urlComponent` | URL Component | string |  |  |  |  |
| `urlcomponentaliases` |  | siteCategory-urlcomponentaliasesCollection |  |  | [`siteCategory-urlcomponentaliasesCollection`](#sitecategory-urlcomponentaliasescollection) |  |
| `website` |  | webSite |  |  | [`webSite`](webSite.md#website) |  |

## siteCategory-currentaudienceCollection

Browser definition `siteCategory-currentaudienceCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | siteCategory-currentaudienceElement[] |  |  | [`siteCategory-currentaudienceElement`](#sitecategory-currentaudienceelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## siteCategory-currentaudienceElement

Browser definition `siteCategory-currentaudienceElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## siteCategory-presentationItemCollection

Browser definition `siteCategory-presentationItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | siteCategory-presentationItemElement[] |  |  | [`siteCategory-presentationItemElement`](#sitecategory-presentationitemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## siteCategory-presentationItemElement

Browser definition `siteCategory-presentationItemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `basePrice` | Base Price | number | double |  |  |  |
| `description` | Item Description | string |  |  |  |  |
| `fileCabinet` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `infoItem` |  | object |  |  |  |  |
| `infoItem.id` | Internal identifier | string |  |  |  |  |
| `infoItem.refName` | Reference Name | string |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemType` |  | object |  |  |  |  |
| `itemType.id` | Internal identifier | string |  |  |  | `FILECABITEM`, `PRESCATEGORY`, `INVTITEM`, `INFOITEM` |
| `itemType.refName` | Reference Name | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `onlinePrice` | Online Price | number | double |  |  |  |
| `presentationItem` | Item | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## siteCategory-tag_subs_machineCollection

Browser definition `siteCategory-tag_subs_machineCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | siteCategory-tag_subs_machineElement[] |  |  | [`siteCategory-tag_subs_machineElement`](#sitecategory-tag_subs_machineelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## siteCategory-tag_subs_machineElement

Browser definition `siteCategory-tag_subs_machineElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `tag` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `value` | Substitution Value | string |  |  |  |  |

## siteCategory-translationsCollection

Browser definition `siteCategory-translationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | siteCategory-translationsElement[] |  |  | [`siteCategory-translationsElement`](#sitecategory-translationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## siteCategory-translationsElement

Browser definition `siteCategory-translationsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Brief Description / Greeting | string |  |  |  |  |
| `displayName` | Name / Title / Category | string |  |  |  |  |
| `language` | Language | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `locale` |  | object |  |  |  |  |
| `locale.id` | Internal identifier | string |  |  |  | `it_CH`, `en_TC`, `af_ZA`, `es_EA`, `es_EC`, `pt_BR`, `en_CY`, `fr_LU`, `nl_AN`, `es_UY`, `en_TT`, `es_ES`, `pt_ST`, `en_DM`, `en_TZ`, `es_ES_EURO`, `fr_ML`, `de_DE_onLQA`, `es_VE`, `nl_BE`, `da_DK`, `pt_AO`, `to_TO`, `en_UG`, `am_ET`, `ss_SZ`, `nl_BQ`, `ar`, `pt_AW`, `ko_KR`, `en_US`, `fr_BE_EURO`, `ko_KP`, `si_AQ`, `fr_MG`, `el_GR`, `be_BY`, `en_AU`, `he_IL`, `en_AW`, `es_SV`, `en_BB`, `ar_YE`, `es_CO`, `es_CL`, `en_BM`, `es_CR`, `pa_IN`, `en_SC`, `en_BS`, `sm_WS`, `it_IT_EURO`, `fr_KM`, `es_CU`, `en_SB`, `en_SG`, `en_BW`, `en_SH`, `en_BZ`, `en_SL`, `az_AZ`, `fi_FI`, `en_SS`, `sr_YU`, `en_CD`, `en_CA`, `ka_GE`, `lv_LV`, `uk_UA`, `es_DO`, `ur_PK`, `ar_IQ`, `fr_LU_EURO`, `pt_PT`, `fr_FR_EURO`, `en_PH`, `th_TH`, `bn_BD`, `si_LK`, `en_PG`, `hu_HU`, `ar_SA`, `ar_SD`, `ru_KZ`, `ar_BH`, `nl_BE_EURO`, `ro_MD`, `en_QA`, `ru_KG`, `es_AR`, `ta_IN`, `sr_RS`, `aa_ER`, `en`, `de_DE_EURO`, `zh_MO`, `en_AE`, `ar_SY`, `es_BO`, `en_AI`, `no_NO`, `en_AG`, `nl_SR`, `fr_VU`, `en_MW`, `gu_AQ`, `ar_TN`, `nl_SX`, `hi_IN`, `en_NA`, `mn_MN`, `en_NG`, `fr_FR`, `ms_MY`, `nl_CW`, `uz_UZ`, `ar_DJ`, `sr_CS`, `de_AT_EURO`, `en_NZ`, `es_PE`, `es_PA`, `fa_IR`, `ar_DZ`, `fr_GN`, `lb_LU`, `xx_US`, `pt_CV`, `sh_RS`, `ht_HT`, `fr_WF`, `es_AR_onLQA`, `es_PR`, `ar_EG`, `es_PY`, `fr_GA`, `en_KW`, `de_AT`, `ro_RO`, `en_KY`, `fr_FR_onLQA`, `fr_DJ`, `ca_ES_EURO`, `cs_CZ`, `en_LC`, `pl_AQ`, `fr_TD`, `fr_TG`, `es_MX`, `sv_AX`, `sk_SK`, `en_LR`, `en_LS`, `ar_OM`, `dz_BT`, `te_IN`, `de_LU_EURO`, `sq_AL`, `sv_SE`, `sn_ZW`, `es_NI`, `en_IE_EURO`, `my_MM`, `en_MF`, `en_MU`, `it_IT`, `pl_PL`, `fr_BE`, `fr_BF`, `tr_TR`, `fr_BI`, `fr_BJ`, `id_ID`, `fr_RW`, `en_ZM`, `km_KH`, `ja_JP`, `de_DE`, `fr_BL`, `tg_TJ`, `ar_QA`, `de_CH`, `zh_HK`, `pt_PT_EURO`, `en_JO`, `en_JM`, `fr_CA`, `nl_NL_EURO`, `fr_CF`, `fr_CG`, `fr_CD`, `pa_AQ`, `fr_CH`, `xx_US_wthId`, `fr_CI`, `pt_GW`, `vi_VN`, `ru_MD`, `fr_CM`, `fr_SC`, `en_KE`, `ne_NP`, `bs_BA`, `sl_SI`, `en_KN`, `fr_SN`, `ar_AE`, `en_GY`, `tl_PH`, `ca_ES`, `es_IC`, `lo_LA`, `kn_IN`, `so_SO`, `fr_PF`, `ar_JO`, `nl_NL`, `is_IS`, `fi_FI_EURO`, `pt_MZ`, `sk_SK_EURO`, `sl_SI_EURO`, `en_IE`, `ms_BN`, `hr_HR`, `ar_KW`, `de_LU`, `lt_LT`, `en_IN`, `ps_AF`, `en_ZA`, `en_VC`, `ru_RU`, `sh_YU`, `ar_LB`, `mr_IN`, `dv_MV`, `fj_FJ`, `zh_TW`, `tk_TM`, `ar_LY`, `en_VU`, `fr_NE`, `en_FK`, `es_GT`, `fr_NC`, `es_GQ`, `fa_AF`, `bg_BG`, `hy_AM`, `en_CY_EURO`, `mk_MK`, `ar_MA`, `en_GD`, `en_GB`, `es_HN`, `gu_IN`, `en_GH`, `et_EE`, `en_GI`, `zh_CN`, `en_GM`, `ar_MR` |
| `locale.refName` | Reference Name | string |  |  |  |  |
| `pageTitle` | Page Title | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `salesdescription` | Detailed Description / Message | string |  |  |  |  |

## siteCategory-urlcomponentaliasesCollection

Browser definition `siteCategory-urlcomponentaliasesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | siteCategory-urlcomponentaliasesElement[] |  |  | [`siteCategory-urlcomponentaliasesElement`](#sitecategory-urlcomponentaliaseselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## siteCategory-urlcomponentaliasesElement

Browser definition `siteCategory-urlcomponentaliasesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `alias` | Alias | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## siteCategoryCollection

Browser definition `siteCategoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | siteCategory[] |  |  | [`siteCategory`](#sitecategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## siteCategorySelectOptions

Browser definition `siteCategorySelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `categoryListLayout` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `correlatedItemsListLayout` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemListLayout` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parentCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `relatedItemsListLayout` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `siteCategoryType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `siteMapPriority` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `storeDisplayImage` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `storeDisplayThumbnail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `website` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

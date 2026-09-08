# Schemas: inventoryStatus

Property tables for definitions owned by `inventoryStatus`.

Record page: [inventoryStatus](../records/inventoryStatus.md).

## Index

- [inventoryStatus](#inventorystatus) — 17 properties
- [inventoryStatus-inventoryBalanceCollection](#inventorystatus-inventorybalancecollection) — 6 properties
- [inventoryStatus-inventoryBalanceElement](#inventorystatus-inventorybalanceelement) — 15 properties
- [inventoryStatus-translationsCollection](#inventorystatus-translationscollection) — 6 properties
- [inventoryStatus-translationsElement](#inventorystatus-translationselement) — 8 properties
- [inventoryStatusCollection](#inventorystatuscollection) — 6 properties
- [inventoryStatusSelectOptions](#inventorystatusselectoptions) — 2 properties

## inventoryStatus

Browser definition `inventoryStatus`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `inventoryAvailForAlloc` | Make Inventory Available For Allocation and Planning | boolean |  |  |  |  |
| `inventoryAvailable` | Make Inventory Available For Commitment | boolean |  |  |  |  |
| `inventoryBalance` |  | inventoryStatus-inventoryBalanceCollection |  |  | [`inventoryStatus-inventoryBalanceCollection`](#inventorystatus-inventorybalancecollection) |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `state` |  | object |  |  |  |  |
| `state.id` | Internal identifier | string |  |  |  | `A`, `D`, `I` |
| `state.refName` | Reference Name | string |  |  |  |  |
| `translations` |  | inventoryStatus-translationsCollection |  |  | [`inventoryStatus-translationsCollection`](#inventorystatus-translationscollection) |  |
| `vendorConsignedStatusType` | Use for Vendor Consigned Inventory | boolean |  |  |  |  |

## inventoryStatus-inventoryBalanceCollection

Browser definition `inventoryStatus-inventoryBalanceCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | inventoryStatus-inventoryBalanceElement[] |  |  | [`inventoryStatus-inventoryBalanceElement`](#inventorystatus-inventorybalanceelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryStatus-inventoryBalanceElement

Browser definition `inventoryStatus-inventoryBalanceElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `binNumber` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `committedQtyPerLocation` | Committed Quantity (Per Location) | string |  |  |  |  |
| `committedQtyPerSerialLotNumber` | Committed Quantity (Per Serial/Lot Number) | string |  |  |  |  |
| `committedQtyPerSerialLotNumberLocation` | Committed Quantity (Per Serial/Lot Number & Location) | string |  |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `inventoryNumber` |  | inventoryNumber |  |  | [`inventoryNumber`](inventoryNumber.md#inventorynumber) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `licensePlateNumber` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantityAvailable` | Available Quantity | string |  |  |  |  |
| `quantityOnHand` | On-Hand Quantity | string |  |  |  |  |
| `quantityPicked` | Picked Quantity | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## inventoryStatus-translationsCollection

Browser definition `inventoryStatus-translationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | inventoryStatus-translationsElement[] |  |  | [`inventoryStatus-translationsElement`](#inventorystatus-translationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryStatus-translationsElement

Browser definition `inventoryStatus-translationsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `description` | Description | string |  |  |  |  |
| `language` | Language | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `locale` |  | object |  |  |  |  |
| `locale.id` | Internal identifier | string |  |  |  | `it_CH`, `en_TC`, `af_ZA`, `es_EA`, `es_EC`, `pt_BR`, `en_CY`, `fr_LU`, `nl_AN`, `es_UY`, `en_TT`, `es_ES`, `pt_ST`, `en_DM`, `en_TZ`, `es_ES_EURO`, `fr_ML`, `de_DE_onLQA`, `es_VE`, `nl_BE`, `da_DK`, `pt_AO`, `to_TO`, `en_UG`, `am_ET`, `ss_SZ`, `nl_BQ`, `ar`, `pt_AW`, `ko_KR`, `en_US`, `fr_BE_EURO`, `ko_KP`, `si_AQ`, `fr_MG`, `el_GR`, `be_BY`, `en_AU`, `he_IL`, `en_AW`, `es_SV`, `en_BB`, `ar_YE`, `es_CO`, `es_CL`, `en_BM`, `es_CR`, `pa_IN`, `en_SC`, `en_BS`, `sm_WS`, `it_IT_EURO`, `fr_KM`, `es_CU`, `en_SB`, `en_SG`, `en_BW`, `en_SH`, `en_BZ`, `en_SL`, `az_AZ`, `fi_FI`, `en_SS`, `sr_YU`, `en_CD`, `en_CA`, `ka_GE`, `lv_LV`, `uk_UA`, `es_DO`, `ur_PK`, `ar_IQ`, `fr_LU_EURO`, `pt_PT`, `fr_FR_EURO`, `en_PH`, `th_TH`, `bn_BD`, `si_LK`, `en_PG`, `hu_HU`, `ar_SA`, `ar_SD`, `ru_KZ`, `ar_BH`, `nl_BE_EURO`, `ro_MD`, `en_QA`, `ru_KG`, `es_AR`, `ta_IN`, `sr_RS`, `aa_ER`, `en`, `de_DE_EURO`, `zh_MO`, `en_AE`, `ar_SY`, `es_BO`, `en_AI`, `no_NO`, `en_AG`, `nl_SR`, `fr_VU`, `en_MW`, `gu_AQ`, `ar_TN`, `nl_SX`, `hi_IN`, `en_NA`, `mn_MN`, `en_NG`, `fr_FR`, `ms_MY`, `nl_CW`, `uz_UZ`, `ar_DJ`, `sr_CS`, `de_AT_EURO`, `en_NZ`, `es_PE`, `es_PA`, `fa_IR`, `ar_DZ`, `fr_GN`, `lb_LU`, `xx_US`, `pt_CV`, `sh_RS`, `ht_HT`, `fr_WF`, `es_AR_onLQA`, `es_PR`, `ar_EG`, `es_PY`, `fr_GA`, `en_KW`, `de_AT`, `ro_RO`, `en_KY`, `fr_FR_onLQA`, `fr_DJ`, `ca_ES_EURO`, `cs_CZ`, `en_LC`, `pl_AQ`, `fr_TD`, `fr_TG`, `es_MX`, `sv_AX`, `sk_SK`, `en_LR`, `en_LS`, `ar_OM`, `dz_BT`, `te_IN`, `de_LU_EURO`, `sq_AL`, `sv_SE`, `sn_ZW`, `es_NI`, `en_IE_EURO`, `my_MM`, `en_MF`, `en_MU`, `it_IT`, `pl_PL`, `fr_BE`, `fr_BF`, `tr_TR`, `fr_BI`, `fr_BJ`, `id_ID`, `fr_RW`, `en_ZM`, `km_KH`, `ja_JP`, `de_DE`, `fr_BL`, `tg_TJ`, `ar_QA`, `de_CH`, `zh_HK`, `pt_PT_EURO`, `en_JO`, `en_JM`, `fr_CA`, `nl_NL_EURO`, `fr_CF`, `fr_CG`, `fr_CD`, `pa_AQ`, `fr_CH`, `xx_US_wthId`, `fr_CI`, `pt_GW`, `vi_VN`, `ru_MD`, `fr_CM`, `fr_SC`, `en_KE`, `ne_NP`, `bs_BA`, `sl_SI`, `en_KN`, `fr_SN`, `ar_AE`, `en_GY`, `tl_PH`, `ca_ES`, `es_IC`, `lo_LA`, `kn_IN`, `so_SO`, `fr_PF`, `ar_JO`, `nl_NL`, `is_IS`, `fi_FI_EURO`, `pt_MZ`, `sk_SK_EURO`, `sl_SI_EURO`, `en_IE`, `ms_BN`, `hr_HR`, `ar_KW`, `de_LU`, `lt_LT`, `en_IN`, `ps_AF`, `en_ZA`, `en_VC`, `ru_RU`, `sh_YU`, `ar_LB`, `mr_IN`, `dv_MV`, `fj_FJ`, `zh_TW`, `tk_TM`, `ar_LY`, `en_VU`, `fr_NE`, `en_FK`, `es_GT`, `fr_NC`, `es_GQ`, `fa_AF`, `bg_BG`, `hy_AM`, `en_CY_EURO`, `mk_MK`, `ar_MA`, `en_GD`, `en_GB`, `es_HN`, `gu_IN`, `en_GH`, `et_EE`, `en_GI`, `zh_CN`, `en_GM`, `ar_MR` |
| `locale.refName` | Reference Name | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## inventoryStatusCollection

Browser definition `inventoryStatusCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | inventoryStatus[] |  |  | [`inventoryStatus`](#inventorystatus) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## inventoryStatusSelectOptions

Browser definition `inventoryStatusSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `state` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

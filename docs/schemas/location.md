# Schemas: location

Property tables for definitions owned by `location`.

Record page: [location](../records/location.md).

## Index

- [location](#location) — 63 properties
- [location-businessHoursCollection](#location-businesshourscollection) — 6 properties
- [location-businessHoursElement](#location-businesshourselement) — 12 properties
- [location-classTranslationCollection](#location-classtranslationcollection) — 6 properties
- [location-classTranslationElement](#location-classtranslationelement) — 7 properties
- [location-docNumberingCollection](#location-docnumberingcollection) — 6 properties
- [location-docNumberingElement](#location-docnumberingelement) — 7 properties
- [location-excludeLocationRegionsCollection](#location-excludelocationregionscollection) — 6 properties
- [location-excludeLocationRegionsElement](#location-excludelocationregionselement) — 5 properties
- [location-includeLocationRegionsCollection](#location-includelocationregionscollection) — 6 properties
- [location-includeLocationRegionsElement](#location-includelocationregionselement) — 5 properties
- [location-inventoryBalanceCollection](#location-inventorybalancecollection) — 6 properties
- [location-inventoryBalanceElement](#location-inventorybalanceelement) — 15 properties
- [location-mainAddress](#location-mainaddress) — 18 properties
- [location-returnAddress](#location-returnaddress) — 18 properties
- [location-tranNumberingCollection](#location-trannumberingcollection) — 6 properties
- [location-tranNumberingElement](#location-trannumberingelement) — 7 properties
- [locationCollection](#locationcollection) — 6 properties
- [locationSelectOptions](#locationselectoptions) — 8 properties

## location

Browser definition `location`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `allowStorePickup` | Allow Store Pickup | boolean |  |  |  |  |
| `autoAssignmentRegionSetting` |  | object |  |  |  |  |
| `autoAssignmentRegionSetting.id` | Internal identifier | string |  |  |  | `0`, `1`, `2`, `3` |
| `autoAssignmentRegionSetting.refName` | Reference Name | string |  |  |  |  |
| `bufferStock` | Buffer Stock | integer | int64 |  |  |  |
| `businessHours` |  | location-businessHoursCollection |  |  | [`location-businessHoursCollection`](#location-businesshourscollection) |  |
| `classTranslation` |  | location-classTranslationCollection |  |  | [`location-classTranslationCollection`](#location-classtranslationcollection) |  |
| `dailyShippingCapacity` | Daily Shipping Capacity | integer | int64 |  |  |  |
| `defaultAllocationPriority` | Default Allocation Priority | number | float |  |  |  |
| `docNumbering` |  | location-docNumberingCollection |  |  | [`location-docNumberingCollection`](#location-docnumberingcollection) |  |
| `excludeLocationRegions` |  | location-excludeLocationRegionsCollection |  |  | [`location-excludeLocationRegionsCollection`](#location-excludelocationregionscollection) |  |
| `externalId` | External ID | string |  |  |  |  |
| `fullName` | Full Name | string |  |  |  |  |
| `geolocationMethod` |  | object |  |  |  |  |
| `geolocationMethod.id` | Internal identifier | string |  |  |  | `POSTALCODE`, `LATLONG` |
| `geolocationMethod.refName` | Reference Name | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `includeChildren` | Include Children | boolean |  |  |  |  |
| `includeInControlTower` | Include In Control Tower | boolean |  |  |  |  |
| `includeInSupplyPlanning` | Include in Supply Planning | boolean |  |  |  |  |
| `includeLocationRegions` |  | location-includeLocationRegionsCollection |  |  | [`location-includeLocationRegionsCollection`](#location-includelocationregionscollection) |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `inventoryBalance` |  | location-inventoryBalanceCollection |  |  | [`location-inventoryBalanceCollection`](#location-inventorybalancecollection) |  |
| `invtTurnoverVelocity` | General inventory turn-over velocity | integer | int64 |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `latitude` | Latitude | number | float |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `locationType` |  | object |  |  |  |  |
| `locationType.id` | Internal identifier | string |  |  |  | `1`, `2` |
| `locationType.refName` | Reference Name | string |  |  |  |  |
| `logo` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `longitude` | Longitude | number | float |  |  |  |
| `mainAddress` |  | location-mainAddress |  |  | [`location-mainAddress`](#location-mainaddress) |  |
| `makeInventoryAvailable` | Make Inventory Available | boolean |  |  |  |  |
| `makeInventoryAvailableStore` | Make Inventory Available in Web Store | boolean |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `nextPickupCutoffTime` | Next Pickup Cut-Off Time | string | date-time |  |  |  |
| `parent` |  | location |  |  | [`location`](#location) |  |
| `pickupAlertEmail` | Email for Store Pickup Alerts | string |  |  |  |  |
| `planningWorkCalendar` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `returnAddress` |  | location-returnAddress |  |  | [`location-returnAddress`](#location-returnaddress) |  |
| `sameDayShipCutOff` | Same day ship cut-off | string |  |  |  |  |
| `soPredConfidence` | Sales Order Predicted Risk Confidence | number | double |  |  |  |
| `soPredictedDays` | Sales Order Predicted Days Late/Early | integer | int64 |  |  |  |
| `storeFulfillmentMemo` | Memo | string |  |  |  |  |
| `storePickupBufferStock` | Store Pickup Buffer Stock | number | float |  |  |  |
| `subsidiary` |  | subsidiaryCollection |  |  | [`subsidiaryCollection`](subsidiary.md#subsidiarycollection) |  |
| `timeZone` |  | object |  |  |  |  |
| `timeZone.id` | Internal identifier | string |  |  |  | `America/Sao_Paulo`, `Asia/Vladivostok`, `Africa/Nairobi`, `Asia/Hong_Kong`, `Asia/Riyadh`, `Pacific/Kwajalein`, `America/Montevideo`, `Africa/Cairo`, `Africa/Windhoek`, `Asia/Karachi`, `Europe/Moscow`, `Pacific/Honolulu`, `America/Guatemala`, `Australia/Hobart`, `Australia/Darwin`, `Australia/Perth`, `Europe/London`, `Asia/Kuala_Lumpur`, `Asia/Baghdad`, `Europe/Budapest`, `Asia/Rangoon`, `America/Bogota`, `America/Manaus`, `Asia/Calcutta`, `America/Tijuana`, `Asia/Kabul`, `Pacific/Tongatapu`, `Europe/Helsinki`, `America/New_York`, `Asia/Beirut`, `Asia/Yerevan`, `Atlantic/Azores`, `Etc/GMT+12`, `America/Chihuahua`, `Asia/Krasnoyarsk`, `GMT`, `America/Anchorage`, `Europe/Warsaw`, `America/Chicago`, `Asia/Yakutsk`, `America/Halifax`, `Etc/GMT-1`, `Africa/Johannesburg`, `America/Godthab`, `Europe/Paris`, `Europe/Istanbul`, `Etc/GMT-3`, `America/Santiago`, `Europe/Minsk`, `Pacific/Auckland`, `Asia/Baku`, `America/Caracas`, `Europe/Kiev`, `Asia/Tehran`, `Asia/Dacca`, `Atlantic/Reykjavik`, `Pacific/Samoa`, `America/La_Paz`, `Asia/Taipei`, `America/Regina`, `Asia/Tashkent`, `Asia/Manila`, `Asia/Bangkok`, `Pacific/Guam`, `Asia/Irkutsk`, `America/St_Johns`, `Asia/Muscat`, `America/Denver`, `US/East-Indiana`, `America/Hermosillo`, `Europe/Amsterdam`, `America/Buenos_Aires`, `America/Noronha`, `Asia/Amman`, `Asia/Seoul`, `Australia/Sydney`, `Asia/Tokyo`, `Australia/Adelaide`, `Asia/Katmandu`, `Asia/Almaty`, `America/Phoenix`, `America/Los_Angeles`, `Australia/Brisbane`, `America/Mexico_City`, `Asia/Yekaterinburg`, `Etc/GMT+3`, `Pacific/Guadalcanal`, `Asia/Jerusalem`, `Etc/GMT+1` |
| `timeZone.refName` | Reference Name | string |  |  |  |  |
| `toPredConfidence` | Transfer Order Predicted Risk Confidence | number | double |  |  |  |
| `toPredictedDays` | Transfer Order Predicted Days Late/Early | integer | int64 |  |  |  |
| `totalShippingCapacity` | Total Shipping Capacity | integer | int64 |  |  |  |
| `tranInternalPrefix` | Transaction Number Prefix | string |  |  |  |  |
| `tranNumbering` |  | location-tranNumberingCollection |  |  | [`location-tranNumberingCollection`](#location-trannumberingcollection) |  |
| `tranPrefix` | Document Number Prefix | string |  |  |  |  |
| `useBins` | Use Bins | boolean |  |  |  |  |
| `useLicensePlates` | Use License Plates | boolean |  |  |  |  |
| `useWarehouseManagement` | Use Warehouse Management | boolean |  |  |  |  |
| `useWorkCalendarForPurchOrder` | Use Work Calendar for Purchase Orders | boolean |  |  |  |  |
| `useWorkCalendarForWorkOrder` | Use Work Calendar for Work Orders | boolean |  |  |  |  |

## location-businessHoursCollection

Browser definition `location-businessHoursCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | location-businessHoursElement[] |  |  | [`location-businessHoursElement`](#location-businesshourselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## location-businessHoursElement

Browser definition `location-businessHoursElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `endTime` | End time | string |  |  |  |  |
| `isFriday` | Friday | boolean |  |  |  |  |
| `isMonday` | Monday | boolean |  |  |  |  |
| `isSaturday` | Saturday | boolean |  |  |  |  |
| `isSunday` | Sunday | boolean |  |  |  |  |
| `isThursday` | Thursday | boolean |  |  |  |  |
| `isTuesday` | Tuesday | boolean |  |  |  |  |
| `isWednesday` | Wednesday | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `sameDayPickupCutOffTime` | Same Day Pickup Cut-Off Time | string |  |  |  |  |
| `startTime` | Start Time | string |  |  |  |  |

## location-classTranslationCollection

Browser definition `location-classTranslationCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | location-classTranslationElement[] |  |  | [`location-classTranslationElement`](#location-classtranslationelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## location-classTranslationElement

Browser definition `location-classTranslationElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `language` | Language | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `locale` |  | object |  |  |  |  |
| `locale.id` | Internal identifier | string |  |  |  | `it_CH`, `en_TC`, `af_ZA`, `es_EA`, `es_EC`, `pt_BR`, `en_CY`, `fr_LU`, `nl_AN`, `es_UY`, `en_TT`, `es_ES`, `pt_ST`, `en_DM`, `en_TZ`, `es_ES_EURO`, `fr_ML`, `de_DE_onLQA`, `es_VE`, `nl_BE`, `da_DK`, `pt_AO`, `to_TO`, `en_UG`, `am_ET`, `ss_SZ`, `nl_BQ`, `ar`, `pt_AW`, `ko_KR`, `en_US`, `fr_BE_EURO`, `ko_KP`, `si_AQ`, `fr_MG`, `el_GR`, `be_BY`, `en_AU`, `he_IL`, `en_AW`, `es_SV`, `en_BB`, `ar_YE`, `es_CO`, `es_CL`, `en_BM`, `es_CR`, `pa_IN`, `en_SC`, `en_BS`, `sm_WS`, `it_IT_EURO`, `fr_KM`, `es_CU`, `en_SB`, `en_SG`, `en_BW`, `en_SH`, `en_BZ`, `en_SL`, `az_AZ`, `fi_FI`, `en_SS`, `sr_YU`, `en_CD`, `en_CA`, `ka_GE`, `lv_LV`, `uk_UA`, `es_DO`, `ur_PK`, `ar_IQ`, `fr_LU_EURO`, `pt_PT`, `fr_FR_EURO`, `en_PH`, `th_TH`, `bn_BD`, `si_LK`, `en_PG`, `hu_HU`, `ar_SA`, `ar_SD`, `ru_KZ`, `ar_BH`, `nl_BE_EURO`, `ro_MD`, `en_QA`, `ru_KG`, `es_AR`, `ta_IN`, `sr_RS`, `aa_ER`, `en`, `de_DE_EURO`, `zh_MO`, `en_AE`, `ar_SY`, `es_BO`, `en_AI`, `no_NO`, `en_AG`, `nl_SR`, `fr_VU`, `en_MW`, `gu_AQ`, `ar_TN`, `nl_SX`, `hi_IN`, `en_NA`, `mn_MN`, `en_NG`, `fr_FR`, `ms_MY`, `nl_CW`, `uz_UZ`, `ar_DJ`, `sr_CS`, `de_AT_EURO`, `en_NZ`, `es_PE`, `es_PA`, `fa_IR`, `ar_DZ`, `fr_GN`, `lb_LU`, `xx_US`, `pt_CV`, `sh_RS`, `ht_HT`, `fr_WF`, `es_AR_onLQA`, `es_PR`, `ar_EG`, `es_PY`, `fr_GA`, `en_KW`, `de_AT`, `ro_RO`, `en_KY`, `fr_FR_onLQA`, `fr_DJ`, `ca_ES_EURO`, `cs_CZ`, `en_LC`, `pl_AQ`, `fr_TD`, `fr_TG`, `es_MX`, `sv_AX`, `sk_SK`, `en_LR`, `en_LS`, `ar_OM`, `dz_BT`, `te_IN`, `de_LU_EURO`, `sq_AL`, `sv_SE`, `sn_ZW`, `es_NI`, `en_IE_EURO`, `my_MM`, `en_MF`, `en_MU`, `it_IT`, `pl_PL`, `fr_BE`, `fr_BF`, `tr_TR`, `fr_BI`, `fr_BJ`, `id_ID`, `fr_RW`, `en_ZM`, `km_KH`, `ja_JP`, `de_DE`, `fr_BL`, `tg_TJ`, `ar_QA`, `de_CH`, `zh_HK`, `pt_PT_EURO`, `en_JO`, `en_JM`, `fr_CA`, `nl_NL_EURO`, `fr_CF`, `fr_CG`, `fr_CD`, `pa_AQ`, `fr_CH`, `xx_US_wthId`, `fr_CI`, `pt_GW`, `vi_VN`, `ru_MD`, `fr_CM`, `fr_SC`, `en_KE`, `ne_NP`, `bs_BA`, `sl_SI`, `en_KN`, `fr_SN`, `ar_AE`, `en_GY`, `tl_PH`, `ca_ES`, `es_IC`, `lo_LA`, `kn_IN`, `so_SO`, `fr_PF`, `ar_JO`, `nl_NL`, `is_IS`, `fi_FI_EURO`, `pt_MZ`, `sk_SK_EURO`, `sl_SI_EURO`, `en_IE`, `ms_BN`, `hr_HR`, `ar_KW`, `de_LU`, `lt_LT`, `en_IN`, `ps_AF`, `en_ZA`, `en_VC`, `ru_RU`, `sh_YU`, `ar_LB`, `mr_IN`, `dv_MV`, `fj_FJ`, `zh_TW`, `tk_TM`, `ar_LY`, `en_VU`, `fr_NE`, `en_FK`, `es_GT`, `fr_NC`, `es_GQ`, `fa_AF`, `bg_BG`, `hy_AM`, `en_CY_EURO`, `mk_MK`, `ar_MA`, `en_GD`, `en_GB`, `es_HN`, `gu_IN`, `en_GH`, `et_EE`, `en_GI`, `zh_CN`, `en_GM`, `ar_MR` |
| `locale.refName` | Reference Name | string |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## location-docNumberingCollection

Browser definition `location-docNumberingCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | location-docNumberingElement[] |  |  | [`location-docNumberingElement`](#location-docnumberingelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## location-docNumberingElement

Browser definition `location-docNumberingElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `advNumLink` | Advanced Numbering | string |  |  |  |  |
| `curNum` | Current Number | string |  |  |  |  |
| `initNum` | Initial Number | string |  |  |  |  |
| `initNumUpdate` | Update Initial Number | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `tranTypeName` | Type | string |  |  |  |  |

## location-excludeLocationRegionsCollection

Browser definition `location-excludeLocationRegionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | location-excludeLocationRegionsElement[] |  |  | [`location-excludeLocationRegionsElement`](#location-excludelocationregionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## location-excludeLocationRegionsElement

Browser definition `location-excludeLocationRegionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Region name | string |  |  |  |  |
| `ranking` | Ranking | integer | int64 |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `region` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## location-includeLocationRegionsCollection

Browser definition `location-includeLocationRegionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | location-includeLocationRegionsElement[] |  |  | [`location-includeLocationRegionsElement`](#location-includelocationregionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## location-includeLocationRegionsElement

Browser definition `location-includeLocationRegionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Region name | string |  |  |  |  |
| `ranking` | Ranking | integer | int64 |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `region` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## location-inventoryBalanceCollection

Browser definition `location-inventoryBalanceCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | location-inventoryBalanceElement[] |  |  | [`location-inventoryBalanceElement`](#location-inventorybalanceelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## location-inventoryBalanceElement

Browser definition `location-inventoryBalanceElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `binNumber` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `committedQtyPerLocation` | Committed Quantity (Per Location) | string |  |  |  |  |
| `committedQtyPerSerialLotNumber` | Committed Quantity (Per Serial/Lot Number) | string |  |  |  |  |
| `committedQtyPerSerialLotNumberLocation` | Committed Quantity (Per Serial/Lot Number & Location) | string |  |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `inventoryNumber` |  | inventoryNumber |  |  | [`inventoryNumber`](inventoryNumber.md#inventorynumber) |  |
| `inventoryStatus` |  | inventoryStatus |  |  | [`inventoryStatus`](inventoryStatus.md#inventorystatus) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `licensePlateNumber` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `quantityAvailable` | Available Quantity | string |  |  |  |  |
| `quantityOnHand` | On-Hand Quantity | string |  |  |  |  |
| `quantityPicked` | Picked Quantity | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## location-mainAddress

Browser definition `location-mainAddress`.

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

## location-returnAddress

Browser definition `location-returnAddress`.

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

## location-tranNumberingCollection

Browser definition `location-tranNumberingCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | location-tranNumberingElement[] |  |  | [`location-tranNumberingElement`](#location-trannumberingelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## location-tranNumberingElement

Browser definition `location-tranNumberingElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `advNumLink` | Advanced Numbering | string |  |  |  |  |
| `curNum` | Current Number | string |  |  |  |  |
| `initNum` | Initial Number | string |  |  |  |  |
| `initNumUpdate` | Update Initial Number | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `tranTypeName` | Type | string |  |  |  |  |

## locationCollection

Browser definition `locationCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | location[] |  |  | [`location`](#location) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## locationSelectOptions

Browser definition `locationSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `autoAssignmentRegionSetting` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `geolocationMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `locationType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `logo` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `planningWorkCalendar` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `timeZone` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

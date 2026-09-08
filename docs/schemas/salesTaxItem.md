# Schemas: salesTaxItem

Property tables for definitions owned by `salesTaxItem`.

Record page: [salesTaxItem](../records/salesTaxItem.md).

## Index

- [salesTaxItem](#salestaxitem) — 40 properties
- [salesTaxItemCollection](#salestaxitemcollection) — 6 properties
- [salesTaxItemSelectOptions](#salestaxitemselectoptions) — 11 properties

## salesTaxItem

Browser definition `salesTaxItem`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `available` |  | object |  |  |  |  |
| `available.id` | Internal identifier | string |  |  |  | `SALE`, `BOTH`, `PURCHASE` |
| `available.refName` | Reference Name | string |  |  |  |  |
| `city` | City | string |  |  |  |  |
| `county` | County | string |  |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `description` | Description | string |  |  |  |  |
| `displayName` | Display Name/Code | string |  |  |  |  |
| `ecCode` | EC Code | boolean |  |  |  |  |
| `effectiveFrom` | Effective From | string | date |  |  |  |
| `excludeFromTaxReports` | Exclude from Tax Report | boolean |  |  |  |  |
| `exempt` | Exempt | boolean |  |  |  |  |
| `export` | Export | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `importantNote` | Important: Once the tax code record has been saved, you cannot change the value in the Tax Type field. | string |  |  |  |  |
| `includeChildren` | Include Children | boolean |  |  |  |  |
| `isDefault` | Default Code | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `itemId` | Name | string |  |  |  |  |
| `itemType` | Item Type | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `name` | Name | string |  |  |  |  |
| `nexusCountry` |  | object |  |  |  |  |
| `nexusCountry.id` | Internal identifier | string |  |  |  | `PR`, `PS`, `PT`, `PW`, `PY`, `QA`, `AB`, `AD`, `AE`, `AF`, `AG`, `AI`, `AL`, `AM`, `AN`, `AO`, `AQ`, `AR`, `AS`, `AT`, `RE`, `AU`, `AW`, `AX`, `AZ`, `RO`, `BA`, `BB`, `RS`, `BD`, `BE`, `RU`, `BF`, `BG`, `RW`, `BH`, `BI`, `BJ`, `BL`, `BM`, `BN`, `BO`, `SA`, `BQ`, `SB`, `BR`, `SC`, `BS`, `SD`, `BT`, `SE`, `BV`, `SG`, `BW`, `SH`, `SI`, `BY`, `SJ`, `BZ`, `SK`, `SL`, `SM`, `SN`, `SO`, `CA`, `SR`, `CC`, `SS`, `CD`, `ST`, `CF`, `SV`, `CG`, `CH`, `SX`, `CI`, `SY`, `SZ`, `CK`, `CL`, `CM`, `CN`, `CO`, `CR`, `TC`, `CS`, `TD`, `CU`, `TF`, `CV`, `TG`, `CW`, `TH`, `CX`, `CY`, `TJ`, `CZ`, `TK`, `TL`, `TM`, `TN`, `TO`, `TR`, `TT`, `DE`, `TV`, `TW`, `DJ`, `TZ`, `DK`, `DM`, `DO`, `UA`, `UG`, `DZ`, `UM`, `EA`, `EC`, `US`, `EE`, `EG`, `EH`, `UY`, `UZ`, `VA`, `ER`, `VC`, `ES`, `ET`, `VE`, `VG`, `VI`, `VN`, `VU`, `FI`, `FJ`, `FK`, `FM`, `FO`, `FR`, `WF`, `GA`, `GB`, `WS`, `GD`, `GE`, `GF`, `GG`, `GH`, `GI`, `GL`, `GM`, `GN`, `GP`, `GQ`, `GR`, `GS`, `GT`, `GU`, `GW`, `GY`, `XK`, `HK`, `HM`, `HN`, `HR`, `HT`, `YE`, `HU`, `IC`, `ID`, `YT`, `IE`, `IL`, `IM`, `IN`, `IO`, `ZA`, `IQ`, `IR`, `IS`, `IT`, `ZM`, `JE`, `ZW`, `JM`, `JO`, `JP`, `KE`, `KG`, `KH`, `KI`, `KM`, `KN`, `KP`, `KR`, `KW`, `KY`, `KZ`, `LA`, `LB`, `LC`, `LI`, `LK`, `LR`, `LS`, `LT`, `LU`, `LV`, `LY`, `MA`, `MC`, `MD`, `ME`, `MF`, `MG`, `MH`, `MK`, `ML`, `MM`, `MN`, `MO`, `MP`, `MQ`, `MR`, `MS`, `MT`, `MU`, `MV`, `MW`, `MX`, `MY`, `MZ`, `NA`, `NC`, `NE`, `NF`, `NG`, `NI`, `NL`, `NO`, `NP`, `NR`, `NU`, `NZ`, `OM`, `PA`, `PE`, `PF`, `PG`, `PH`, `PK`, `PL`, `PM`, `PN` |
| `nexusCountry.refName` | Reference Name | string |  |  |  |  |
| `parent` |  | salesTaxItem |  |  | [`salesTaxItem`](#salestaxitem) |  |
| `purchaseAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `rate` | Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reverseCharge` | Reverse Charge Code | boolean |  |  |  |  |
| `saleAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `service` | Applies To Service Items | boolean |  |  |  |  |
| `state` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `subsidiary` |  | subsidiaryCollection |  |  | [`subsidiaryCollection`](subsidiary.md#subsidiarycollection) |  |
| `taxAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `taxAgency` |  | vendor |  |  | [`vendor`](vendor.md#vendor) |  |
| `taxType` |  | taxType |  |  | [`taxType`](taxType.md#taxtype) |  |
| `validUntil` | Valid Until | string | date |  |  |  |
| `zip` | Zip Codes | string |  |  |  |  |

## salesTaxItemCollection

Browser definition `salesTaxItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | salesTaxItem[] |  |  | [`salesTaxItem`](#salestaxitem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## salesTaxItemSelectOptions

Browser definition `salesTaxItemSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `available` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nexusCountry` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `purchaseAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `saleAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `state` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxAgency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

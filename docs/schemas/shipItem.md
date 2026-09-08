# Schemas: shipItem

Property tables for definitions owned by `shipItem`.

Record page: [shipItem](../records/shipItem.md).

## Index

- [shipItem](#shipitem) — 160 properties
- [shipItem-handlingTableCollection](#shipitem-handlingtablecollection) — 6 properties
- [shipItem-handlingTableElement](#shipitem-handlingtableelement) — 4 properties
- [shipItem-itemsCollection](#shipitem-itemscollection) — 6 properties
- [shipItem-itemsElement](#shipitem-itemselement) — 4 properties
- [shipItem-shipMethodRuleRelationsCollection](#shipitem-shipmethodrulerelationscollection) — 6 properties
- [shipItem-shipMethodRuleRelationsElement](#shipitem-shipmethodrulerelationselement) — 4 properties
- [shipItem-shippingTableCollection](#shipitem-shippingtablecollection) — 6 properties
- [shipItem-shippingTableElement](#shipitem-shippingtableelement) — 4 properties
- [shipItem-translationsCollection](#shipitem-translationscollection) — 6 properties
- [shipItem-translationsElement](#shipitem-translationselement) — 5 properties
- [shipItemCollection](#shipitemcollection) — 6 properties
- [shipItemSelectOptions](#shipitemselectoptions) — 37 properties

## shipItem

Browser definition `shipItem`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accChange` | Account Change | boolean |  |  |  |  |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `accountHandling` |  | account |  |  | [`account`](account.md#account) |  |
| `costBasis` |  | object |  |  |  |  |
| `costBasis.id` | Internal identifier | string |  |  |  | `pluginRate`, `fedexRealTimeRate`, `upsRealTimeRate`, `uspsRealTimeRate`, `fr`, `weight`, `peritem`, `ptotal`, `shippingtable` |
| `costBasis.refName` | Reference Name | string |  |  |  |  |
| `countries` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `description` | Description | string |  |  |  |  |
| `displayName` | Display Name/Code | string |  |  |  |  |
| `doIfArrangement` | Web Site Rules | string |  |  |  |  |
| `doIfTotal` | Web Site Visibility Limited by Total | boolean |  |  |  |  |
| `doIfTotalAmt` | Web Site Visibility By Total Limit | number | double |  |  |  |
| `doIfTotalOperator` |  | object |  |  |  |  |
| `doIfTotalOperator.id` | Internal identifier | string |  |  |  | `OVER`, `UNDER` |
| `doIfTotalOperator.refName` | Reference Name | string |  |  |  |  |
| `doIfWeight` | Web Site Visibility Limited by Weight | boolean |  |  |  |  |
| `doIfWeightAmt` | Web Site Visibility By Weight Limit | number | float |  |  |  |
| `doIfWeightOperator` |  | object |  |  |  |  |
| `doIfWeightOperator.id` | Internal identifier | string |  |  |  | `OVER`, `UNDER` |
| `doIfWeightOperator.refName` | Reference Name | string |  |  |  |  |
| `doIfWeightUnit` |  | object |  |  |  |  |
| `doIfWeightUnit.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `doIfWeightUnit.refName` | Reference Name | string |  |  |  |  |
| `edition` | Edition | string |  |  |  |  |
| `enabletransittime` | Enable transit time | boolean |  |  |  |  |
| `excludeCountries` | Excluded For Countries | boolean |  |  |  |  |
| `excludeSites` | Excluded For Sites | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fedexDiscountRate` | Discount Rate | number | float |  |  |  |
| `fedexOneRate` | FedEx One Rate® | boolean |  |  |  |  |
| `fedexServiceCode` |  | object |  |  |  |  |
| `fedexServiceCode.id` | Internal identifier | string |  |  |  | `44`, `45`, `46`, `47`, `48`, `49`, `50`, `51`, `52`, `53`, `10`, `54`, `11`, `55`, `12`, `56`, `13`, `57`, `14`, `58`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21`, `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `32`, `33`, `34`, `35`, `36`, `37`, `38`, `40`, `41`, `42`, `43` |
| `fedexServiceCode.refName` | Reference Name | string |  |  |  |  |
| `freeIfOrderTotalIsOverAmount` | Free If Total Over Amount | number | double |  |  |  |
| `handlingAsPercentageOfTotal` | Handling Rate As Percent of Total | number | double |  |  |  |
| `handlingByWeightAmount` | Handling Rate By Weight | number | double |  |  |  |
| `handlingByWeightPerQuantity` | Handling Rate By Weight Per | number | float |  |  |  |
| `handlingByWeightPerUnit` |  | object |  |  |  |  |
| `handlingByWeightPerUnit.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `handlingByWeightPerUnit.refName` | Reference Name | string |  |  |  |  |
| `handlingCost` |  | object |  |  |  |  |
| `handlingCost.id` | Internal identifier | string |  |  |  | `no_handling`, `fr`, `weight`, `peritem`, `ptotal`, `handlingtable` |
| `handlingCost.refName` | Reference Name | string |  |  |  |  |
| `handlingFlatRateAmount` | Handling Flat Rate | number | double |  |  |  |
| `handlingPerItemAmount` | Handling Rate By Item | number | double |  |  |  |
| `handlingTable` |  | shipItem-handlingTableCollection |  |  | [`shipItem-handlingTableCollection`](#shipitem-handlingtablecollection) |  |
| `handlingTableChargeBy` |  | object |  |  |  |  |
| `handlingTableChargeBy.id` | Internal identifier | string |  |  |  | `ORDERTOTAL`, `WEIGHT` |
| `handlingTableChargeBy.refName` | Reference Name | string |  |  |  |  |
| `handlingTableUOM` |  | object |  |  |  |  |
| `handlingTableUOM.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `handlingTableUOM.refName` | Reference Name | string |  |  |  |  |
| `handlingTaxCode` |  | salesTaxItem |  |  | [`salesTaxItem`](salesTaxItem.md#salestaxitem) |  |
| `hasMaximumShippingCost` | Has Maximum Shipping Cost | boolean |  |  |  |  |
| `hasMinimumShippingCost` | Has Minimum Shipping Cost | boolean |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `integratedLabelsArrangement` | Integrated Labels | string |  |  |  |  |
| `integrationServiceCode` |  | object |  |  |  |  |
| `integrationServiceCode.id` | Internal identifier | string |  |  |  | `44`, `45`, `46`, `47`, `48`, `49`, `50`, `51`, `52`, `53`, `10`, `54`, `11`, `55`, `12`, `56`, `13`, `57`, `14`, `58`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21`, `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `32`, `33`, `34`, `35`, `36`, `37`, `38`, `40`, `41`, `42`, `43` |
| `integrationServiceCode.refName` | Reference Name | string |  |  |  |  |
| `invt_DispName` | Display Name | string |  |  |  |  |
| `isFreeIfOrderTotalIsOver` | Is Free If Total Over | boolean |  |  |  |  |
| `isHandlingByWeightBracketed` | Handling Rate By Weight Bracketed | boolean |  |  |  |  |
| `isHandlingTaxable` | Charge Tax on this handling portion of item | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isOnline` | Display in Website | boolean |  |  |  |  |
| `isShippingByWeightBracketed` | Shipping Rate By Weight Bracketed | boolean |  |  |  |  |
| `isTaxable` | Charge Tax on this shipping portion of item | boolean |  |  |  |  |
| `itemId` | Ship Name | string |  |  |  |  |
| `itemType` | stype | string |  |  |  |  |
| `items` |  | shipItem-itemsCollection |  |  | [`shipItem-itemsCollection`](#shipitem-itemscollection) |  |
| `labelPlugin` | Shipping Partner Label | string |  |  |  |  |
| `labelPluginSelect` |  | object |  |  |  |  |
| `labelPluginSelect.id` | Internal identifier | string |  |  |  |  |
| `labelPluginSelect.refName` | Reference Name | string |  |  |  |  |
| `labelReg` | Registration | string |  |  |  |  |
| `labelRegSelect` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `labelService` | Label Service | string |  |  |  |  |
| `labelServiceGroup` | Label Service Group | string |  |  |  |  |
| `labelServiceGroupSelect` |  | object |  |  |  |  |
| `labelServiceGroupSelect.id` | Internal identifier | string |  |  |  |  |
| `labelServiceGroupSelect.refName` | Reference Name | string |  |  |  |  |
| `labelServiceSelect` |  | object |  |  |  |  |
| `labelServiceSelect.id` | Internal identifier | string |  |  |  |  |
| `labelServiceSelect.refName` | Reference Name | string |  |  |  |  |
| `labelType` |  | object |  |  |  |  |
| `labelType.id` | Internal identifier | string |  |  |  |  |
| `labelType.refName` | Reference Name | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `maximumShippingCost` | Maximum Shipping Cost | number | double |  |  |  |
| `minimumShippingCost` | Minimum Shipping Cost | number | double |  |  |  |
| `needsAllFreeShippingItems` | All items must be purchased | boolean |  |  |  |  |
| `omitPackaging` | Omit packaging | boolean |  |  |  |  |
| `pluginLabelsArrangement` | Shipping Partner Labels | string |  |  |  |  |
| `pluginRateArrangement` | Shipping Partner Rate | string |  |  |  |  |
| `ratingPlugin` | Rating Shipping Partner | string |  |  |  |  |
| `ratingPluginSelect` |  | object |  |  |  |  |
| `ratingPluginSelect.id` | Internal identifier | string |  |  |  |  |
| `ratingPluginSelect.refName` | Reference Name | string |  |  |  |  |
| `ratingReg` | Shipping Partner Rate Registration | string |  |  |  |  |
| `ratingRegSelect` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `ratingService` | Rating Service | string |  |  |  |  |
| `ratingServiceGroup` | Rating Service Group | string |  |  |  |  |
| `ratingServiceGroupSelect` |  | object |  |  |  |  |
| `ratingServiceGroupSelect.id` | Internal identifier | string |  |  |  |  |
| `ratingServiceGroupSelect.refName` | Reference Name | string |  |  |  |  |
| `ratingServiceSelect` |  | object |  |  |  |  |
| `ratingServiceSelect.id` | Internal identifier | string |  |  |  |  |
| `ratingServiceSelect.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `restrictionArrangement` | Shipping Restrictions | string |  |  |  |  |
| `returnLabelReg` | Registration | string |  |  |  |  |
| `returnLabelRegSelect` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `returnLabelService` | Label Return Service | string |  |  |  |  |
| `returnLabelServiceSelect` |  | object |  |  |  |  |
| `returnLabelServiceSelect.id` | Internal identifier | string |  |  |  |  |
| `returnLabelServiceSelect.refName` | Reference Name | string |  |  |  |  |
| `returnServiceCode` |  | object |  |  |  |  |
| `returnServiceCode.id` | Internal identifier | string |  |  |  | `44`, `45`, `46`, `47`, `48`, `49`, `50`, `51`, `52`, `53`, `10`, `54`, `11`, `55`, `12`, `56`, `13`, `57`, `14`, `58`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21`, `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `32`, `33`, `34`, `35`, `36`, `37`, `38`, `40`, `41`, `42`, `43` |
| `returnServiceCode.refName` | Reference Name | string |  |  |  |  |
| `returnsIntegrated` | Return Label Integration | boolean |  |  |  |  |
| `shipItemCurrency` | Currency | string |  |  |  |  |
| `shipMethodRuleRelations` |  | shipItem-shipMethodRuleRelationsCollection |  |  | [`shipItem-shipMethodRuleRelationsCollection`](#shipitem-shipmethodrulerelationscollection) |  |
| `shipperIntegrated` | Shipping Label Integration | boolean |  |  |  |  |
| `shippingAsPercentageOfTotal` | Shipping Rate As Percent of Total | number | double |  |  |  |
| `shippingByWeightAmount` | Shipping Rate By Weight | number | double |  |  |  |
| `shippingByWeightPerQuantity` | Shipping Rate By Weight Per | number | float |  |  |  |
| `shippingByWeightPerUnit` |  | object |  |  |  |  |
| `shippingByWeightPerUnit.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `shippingByWeightPerUnit.refName` | Reference Name | string |  |  |  |  |
| `shippingCarrier` | Shipping Carrier | string |  |  |  |  |
| `shippingFlatRateAmount` | Shipping Flat Rate | number | double |  |  |  |
| `shippingPerItemAmount` | Shipping Rate By Item | number | double |  |  |  |
| `shippingTable` |  | shipItem-shippingTableCollection |  |  | [`shipItem-shippingTableCollection`](#shipitem-shippingtablecollection) |  |
| `shippingTableChargeBy` |  | object |  |  |  |  |
| `shippingTableChargeBy.id` | Internal identifier | string |  |  |  | `ORDERTOTAL`, `WEIGHT` |
| `shippingTableChargeBy.refName` | Reference Name | string |  |  |  |  |
| `shippingTableUom` |  | object |  |  |  |  |
| `shippingTableUom.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `shippingTableUom.refName` | Reference Name | string |  |  |  |  |
| `shippingTaxCode` |  | salesTaxItem |  |  | [`salesTaxItem`](salesTaxItem.md#salestaxitem) |  |
| `site` |  | webSiteCollection |  |  | [`webSiteCollection`](webSite.md#websitecollection) |  |
| `states` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `tabText` | Tab Text | string |  |  |  |  |
| `tabpromisingtext` |  | string |  |  |  |  |
| `taxSchedule` |  | taxSchedule |  |  | [`taxSchedule`](taxSchedule.md#taxschedule) |  |
| `taxScheduleHandling` |  | taxSchedule |  |  | [`taxSchedule`](taxSchedule.md#taxschedule) |  |
| `transittimedays` | Transit Time Days | integer | int64 |  |  |  |
| `transittimedayslabel` |  | string |  |  |  |  |
| `translations` |  | shipItem-translationsCollection |  |  | [`shipItem-translationsCollection`](#shipitem-translationscollection) |  |
| `upsDiscountRate` | Discount Rate | number | float |  |  |  |
| `upsSaverName` | UPS Saver Name | string |  |  |  |  |
| `upsServiceCode` |  | object |  |  |  |  |
| `upsServiceCode.id` | Internal identifier | string |  |  |  | `44`, `45`, `46`, `47`, `48`, `49`, `50`, `51`, `52`, `53`, `10`, `54`, `11`, `55`, `12`, `56`, `13`, `57`, `14`, `58`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21`, `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `32`, `33`, `34`, `35`, `36`, `37`, `38`, `40`, `41`, `42`, `43` |
| `upsServiceCode.refName` | Reference Name | string |  |  |  |  |
| `uspsDiscountRate` | Discount Rate | number | float |  |  |  |
| `uspsServiceCode` |  | object |  |  |  |  |
| `uspsServiceCode.id` | Internal identifier | string |  |  |  | `44`, `45`, `46`, `47`, `48`, `49`, `50`, `51`, `52`, `53`, `10`, `54`, `11`, `55`, `12`, `56`, `13`, `57`, `14`, `58`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21`, `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `32`, `33`, `34`, `35`, `36`, `37`, `38`, `40`, `41`, `42`, `43` |
| `uspsServiceCode.refName` | Reference Name | string |  |  |  |  |

## shipItem-handlingTableCollection

Browser definition `shipItem-handlingTableCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | shipItem-handlingTableElement[] |  |  | [`shipItem-handlingTableElement`](#shipitem-handlingtableelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## shipItem-handlingTableElement

Browser definition `shipItem-handlingTableElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `handlingTableCharge` | Charge | number | double |  |  |  |
| `handlingTableRangeValue` | Range Value | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## shipItem-itemsCollection

Browser definition `shipItem-itemsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | shipItem-itemsElement[] |  |  | [`shipItem-itemsElement`](#shipitem-itemselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## shipItem-itemsElement

Browser definition `shipItem-itemsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `nQty` | Quantity | integer | int64 |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## shipItem-shipMethodRuleRelationsCollection

Browser definition `shipItem-shipMethodRuleRelationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | shipItem-shipMethodRuleRelationsElement[] |  |  | [`shipItem-shipMethodRuleRelationsElement`](#shipitem-shipmethodrulerelationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## shipItem-shipMethodRuleRelationsElement

Browser definition `shipItem-shipMethodRuleRelationsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `item` |  | shipItem |  |  | [`shipItem`](#shipitem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |

## shipItem-shippingTableCollection

Browser definition `shipItem-shippingTableCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | shipItem-shippingTableElement[] |  |  | [`shipItem-shippingTableElement`](#shipitem-shippingtableelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## shipItem-shippingTableElement

Browser definition `shipItem-shippingTableElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `shippingTableCharge` | Charge | number | double |  |  |  |
| `shippingTableRangeValue` | Range Value | number | double |  |  |  |

## shipItem-translationsCollection

Browser definition `shipItem-translationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | shipItem-translationsElement[] |  |  | [`shipItem-translationsElement`](#shipitem-translationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## shipItem-translationsElement

Browser definition `shipItem-translationsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `displayName` | Display Name | string |  |  |  |  |
| `language` | Language | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `locale` |  | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## shipItemCollection

Browser definition `shipItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | shipItem[] |  |  | [`shipItem`](#shipitem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## shipItemSelectOptions

Browser definition `shipItemSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `accountHandling` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `costBasis` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `countries` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `doIfTotalOperator` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `doIfWeightOperator` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `doIfWeightUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `fedexServiceCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `handlingByWeightPerUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `handlingCost` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `handlingTableChargeBy` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `handlingTableUOM` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `handlingTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `integrationServiceCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `labelPluginSelect` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `labelRegSelect` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `labelServiceGroupSelect` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `labelServiceSelect` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `labelType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `ratingPluginSelect` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `ratingRegSelect` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `ratingServiceGroupSelect` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `ratingServiceSelect` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `returnLabelRegSelect` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `returnLabelServiceSelect` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `returnServiceCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shippingByWeightPerUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shippingTableChargeBy` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shippingTableUom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shippingTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `site` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `states` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxScheduleHandling` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `upsServiceCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `uspsServiceCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

# Schemas: promotionCode

Property tables for definitions owned by `promotionCode`.

Record page: [promotionCode](../records/promotionCode.md).

## Index

- [promotionCode](#promotioncode) — 71 properties
- [promotionCode-currencyCollection](#promotioncode-currencycollection) — 6 properties
- [promotionCode-currencyElement](#promotioncode-currencyelement) — 4 properties
- [promotionCode-discountedItemsCollection](#promotioncode-discounteditemscollection) — 6 properties
- [promotionCode-discountedItemsElement](#promotioncode-discounteditemselement) — 3 properties
- [promotionCode-itemsCollection](#promotioncode-itemscollection) — 6 properties
- [promotionCode-itemsElement](#promotioncode-itemselement) — 3 properties
- [promotionCode-partnersCollection](#promotioncode-partnerscollection) — 6 properties
- [promotionCode-partnersElement](#promotioncode-partnerselement) — 3 properties
- [promotionCodeCollection](#promotioncodecollection) — 6 properties
- [promotionCodeSelectOptions](#promotioncodeselectoptions) — 20 properties

## promotionCode

Browser definition `promotionCode`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `applyDiscountTo` |  | object |  |  |  |  |
| `applyDiscountTo.id` | Internal identifier | string |  |  |  | `FIRSTSALE`, `ALLSALES` |
| `applyDiscountTo.refName` | Reference Name | string |  |  |  |  |
| `applyDiscountToType` |  | object |  |  |  |  |
| `applyDiscountToType.id` | Internal identifier | string |  |  |  | `MOSTEXPENSIVEDISCITEM`, `CHEAPESTDISCITEM`, `EACHDISCITEM` |
| `applyDiscountToType.refName` | Reference Name | string |  |  |  |  |
| `audience` |  | object |  |  |  |  |
| `audience.id` | Internal identifier | string |  |  |  | `EVERYONE`, `SPECIFICCUSTOMERS` |
| `audience.refName` | Reference Name | string |  |  |  |  |
| `canBeAutoApplied` | Can be Automatically Applied | boolean |  |  |  |  |
| `cannotBeCombined` | Exclusive Promotion | boolean |  |  |  |  |
| `code` | Coupon Code | string |  |  |  |  |
| `codePattern` | Code Pattern | string |  |  |  |  |
| `combinationType` |  | object |  |  |  |  |
| `combinationType.id` | Internal identifier | string |  |  |  | `COMBINABLE`, `GLOBALEXCLUSIVE`, `ITEMLINEEXCLUSIVE`, `ORDERTYPEEXCLUSIVE`, `SHIPPINGTYPEEXCLUSIVE` |
| `combinationType.refName` | Reference Name | string |  |  |  |  |
| `currency` |  | promotionCode-currencyCollection |  |  | [`promotionCode-currencyCollection`](#promotioncode-currencycollection) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `customerCategory` |  | customerCategoryCollection |  |  | [`customerCategoryCollection`](customerCategory.md#customercategorycollection) |  |
| `customerGroup` |  | entityGroup |  |  | [`entityGroup`](entityGroup.md#entitygroup) |  |
| `customerGroupPreference` |  | object |  |  |  |  |
| `customerGroupPreference.id` | Internal identifier | string |  |  |  | `USECACHED`, `RUNEACHTIME` |
| `customerGroupPreference.refName` | Reference Name | string |  |  |  |  |
| `customers` |  | customerCollection |  |  | [`customerCollection`](customer.md#customercollection) |  |
| `description` | Description | string |  |  |  |  |
| `discount` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `discountType` |  | object |  |  |  |  |
| `discountType.id` | Internal identifier | string |  |  |  | `F`, `T` |
| `discountType.refName` | Reference Name | string |  |  |  |  |
| `discountedItems` |  | promotionCode-discountedItemsCollection |  |  | [`promotionCode-discountedItemsCollection`](#promotioncode-discounteditemscollection) |  |
| `discountedItemsSavedSearch` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `displayLineDiscounts` | Display Line Discounts | boolean |  |  |  |  |
| `endDate` | End Date | string | date |  |  |  |
| `excludeItems` | Exclude Items | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fixedPrice` | Fixed Price | number | double |  |  |  |
| `freeShipMethod` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
| `id` | Internal ID | string |  |  |  |  |
| `implementation` |  | object |  |  |  |  |
| `implementation.id` | Internal identifier | string |  |  |  | `default`, `CUSTOMSCRIPT_ADVPROMO_BUYX_GETY`, `CUSTOMSCRIPT_ADVPROMO_ORDER_SPECIFIC`, `CUSTOMSCRIPT_ADVPROMO_ITEM_SPECIFIC` |
| `implementation.refName` | Reference Name | string |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isPublic` | Available to all Customers | boolean |  |  |  |  |
| `itemQuantifier` | Item Quantity | integer | int64 |  |  |  |
| `items` |  | promotionCode-itemsCollection |  |  | [`promotionCode-itemsCollection`](#promotioncode-itemscollection) |  |
| `itemsSavedSearch` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `lastModifiedDate` | Last Modified Date | string | date |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | locationCollection |  |  | [`locationCollection`](location.md#locationcollection) |  |
| `minimumOrderAmount` |  | number | double |  |  |  |
| `minimumOrderAmountCheck` | Minimum Order Amount | boolean |  |  |  |  |
| `name` | Name | string |  |  |  |  |
| `numberToGenerate` | Codes to Generate | integer | int64 |  |  |  |
| `partnerCnt` |  | integer | int64 |  |  |  |
| `partners` |  | promotionCode-partnersCollection |  |  | [`promotionCode-partnersCollection`](#promotioncode-partnerscollection) |  |
| `rate` | Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `repeatDiscount` | Repeat discount incrementally | boolean |  |  |  |  |
| `salesChannels` |  | object |  |  |  |  |
| `salesChannels.id` | Internal identifier | string |  |  |  | `ALL`, `SPECIFICLOCATIONS`, `SPECIFICWEBSITES` |
| `salesChannels.refName` | Reference Name | string |  |  |  |  |
| `specificItemsCheck` | Specific Items | boolean |  |  |  |  |
| `startDate` | Start Date | string | date |  |  |  |
| `useCachedCustomerGroup` | Use Cached Customer Group | boolean |  |  |  |  |
| `useType` |  | object |  |  |  |  |
| `useType.id` | Internal identifier | string |  |  |  | `MULTIPLEUSES`, `SINGLEUSE` |
| `useType.refName` | Reference Name | string |  |  |  |  |
| `website` |  | webSiteCollection |  |  | [`webSiteCollection`](webSite.md#websitecollection) |  |
| `whatTheCustomerNeedsToBuy` |  | object |  |  |  |  |
| `whatTheCustomerNeedsToBuy.id` | Internal identifier | string |  |  |  | `ANYTHING`, `MINIMUMORDERAMOUNTORSPECIFICITEMS` |
| `whatTheCustomerNeedsToBuy.refName` | Reference Name | string |  |  |  |  |

## promotionCode-currencyCollection

Browser definition `promotionCode-currencyCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | promotionCode-currencyElement[] |  |  | [`promotionCode-currencyElement`](#promotioncode-currencyelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## promotionCode-currencyElement

Browser definition `promotionCode-currencyElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `minimumOrderAmount` | Value | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## promotionCode-discountedItemsCollection

Browser definition `promotionCode-discountedItemsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | promotionCode-discountedItemsElement[] |  |  | [`promotionCode-discountedItemsElement`](#promotioncode-discounteditemselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## promotionCode-discountedItemsElement

Browser definition `promotionCode-discountedItemsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `discountedItem` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## promotionCode-itemsCollection

Browser definition `promotionCode-itemsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | promotionCode-itemsElement[] |  |  | [`promotionCode-itemsElement`](#promotioncode-itemselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## promotionCode-itemsElement

Browser definition `promotionCode-itemsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## promotionCode-partnersCollection

Browser definition `promotionCode-partnersCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | promotionCode-partnersElement[] |  |  | [`promotionCode-partnersElement`](#promotioncode-partnerselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## promotionCode-partnersElement

Browser definition `promotionCode-partnersElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `partner` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `refName` | Reference Name | string |  |  |  |  |

## promotionCodeCollection

Browser definition `promotionCodeCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | promotionCode[] |  |  | [`promotionCode`](#promotioncode) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## promotionCodeSelectOptions

Browser definition `promotionCodeSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `applyDiscountTo` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `applyDiscountToType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `audience` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `combinationType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customerCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customerGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customerGroupPreference` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customers` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `discount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `discountType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `discountedItemsSavedSearch` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `freeShipMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `implementation` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemsSavedSearch` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesChannels` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `useType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `website` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `whatTheCustomerNeedsToBuy` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

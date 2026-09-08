# Schemas: nonInventorySaleItem

Property tables for definitions owned by `nonInventorySaleItem`.

Record page: [nonInventorySaleItem](../records/nonInventorySaleItem.md).

## Index

- [nonInventorySaleItem](#noninventorysaleitem) — 191 properties
- [nonInventorySaleItem-accountingBookDetailCollection](#noninventorysaleitem-accountingbookdetailcollection) — 6 properties
- [nonInventorySaleItem-accountingBookDetailElement](#noninventorysaleitem-accountingbookdetailelement) — 11 properties
- [nonInventorySaleItem-correlatedItemsCollection](#noninventorysaleitem-correlateditemscollection) — 6 properties
- [nonInventorySaleItem-correlatedItemsElement](#noninventorysaleitem-correlateditemselement) — 7 properties
- [nonInventorySaleItem-hierarchyVersionsCollection](#noninventorysaleitem-hierarchyversionscollection) — 6 properties
- [nonInventorySaleItem-hierarchyVersionsElement](#noninventorysaleitem-hierarchyversionselement) — 7 properties
- [nonInventorySaleItem-presentationItemCollection](#noninventorysaleitem-presentationitemcollection) — 6 properties
- [nonInventorySaleItem-presentationItemElement](#noninventorysaleitem-presentationitemelement) — 11 properties
- [nonInventorySaleItem-price](#noninventorysaleitem-price) — 6 properties
- [nonInventorySaleItem-priceElement](#noninventorysaleitem-priceelement) — 10 properties
- [nonInventorySaleItem-siteCategoryCollection](#noninventorysaleitem-sitecategorycollection) — 6 properties
- [nonInventorySaleItem-siteCategoryElement](#noninventorysaleitem-sitecategoryelement) — 4 properties
- [nonInventorySaleItem-translationsCollection](#noninventorysaleitem-translationscollection) — 6 properties
- [nonInventorySaleItem-translationsElement](#noninventorysaleitem-translationselement) — 16 properties
- [nonInventorySaleItemCollection](#noninventorysaleitemcollection) — 6 properties
- [nonInventorySaleItemSelectOptions](#noninventorysaleitemselectoptions) — 56 properties

## nonInventorySaleItem

Browser definition `nonInventorySaleItem`.

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
| `accountingBookDetail` |  | nonInventorySaleItem-accountingBookDetailCollection |  |  | [`nonInventorySaleItem-accountingBookDetailCollection`](#noninventorysaleitem-accountingbookdetailcollection) |  |
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
| `correlatedItems` |  | nonInventorySaleItem-correlatedItemsCollection |  |  | [`nonInventorySaleItem-correlatedItemsCollection`](#noninventorysaleitem-correlateditemscollection) |  |
| `costCategory` |  | costCategory |  |  | [`costCategory`](costCategory.md#costcategory) |  |
| `costEstimate` | Item Defined Cost | number | double |  |  |  |
| `costEstimateUnits` | Est. Cost Unit | string |  |  |  |  |
| `costForPricing` | Cost for Pricing | number | double |  |  |  |
| `countryOfManufacture` |  | object |  |  |  |  |
| `countryOfManufacture.id` | Internal identifier | string |  |  |  | `PR`, `PS`, `PT`, `PW`, `PY`, `QA`, `AB`, `AD`, `AE`, `AF`, `AG`, `AI`, `AL`, `AM`, `AN`, `AO`, `AQ`, `AR`, `AS`, `AT`, `RE`, `AU`, `AW`, `AX`, `AZ`, `RO`, `BA`, `BB`, `RS`, `BD`, `BE`, `RU`, `BF`, `BG`, `RW`, `BH`, `BI`, `BJ`, `BL`, `BM`, `BN`, `BO`, `SA`, `BQ`, `SB`, `BR`, `SC`, `BS`, `SD`, `BT`, `SE`, `BV`, `SG`, `BW`, `SH`, `SI`, `BY`, `SJ`, `BZ`, `SK`, `SL`, `SM`, `SN`, `SO`, `CA`, `SR`, `CC`, `SS`, `CD`, `ST`, `CF`, `SV`, `CG`, `CH`, `SX`, `CI`, `SY`, `SZ`, `CK`, `CL`, `CM`, `CN`, `CO`, `CR`, `TC`, `CS`, `TD`, `CU`, `TF`, `CV`, `TG`, `CW`, `TH`, `CX`, `CY`, `TJ`, `CZ`, `TK`, `TL`, `TM`, `TN`, `TO`, `TR`, `TT`, `DE`, `TV`, `TW`, `DJ`, `TZ`, `DK`, `DM`, `DO`, `UA`, `UG`, `DZ`, `UM`, `EA`, `EC`, `US`, `EE`, `EG`, `EH`, `UY`, `UZ`, `VA`, `ER`, `VC`, `ES`, `ET`, `VE`, `VG`, `VI`, `VN`, `VU`, `FI`, `FJ`, `FK`, `FM`, `FO`, `FR`, `WF`, `GA`, `GB`, `WS`, `GD`, `GE`, `GF`, `GG`, `GH`, `GI`, `GL`, `GM`, `GN`, `GP`, `GQ`, `GR`, `GS`, `GT`, `GU`, `GW`, `GY`, `XK`, `HK`, `HM`, `HN`, `HR`, `HT`, `YE`, `HU`, `IC`, `ID`, `YT`, `IE`, `IL`, `IM`, `IN`, `IO`, `ZA`, `IQ`, `IR`, `IS`, `IT`, `ZM`, `JE`, `ZW`, `JM`, `JO`, `JP`, `KE`, `KG`, `KH`, `KI`, `KM`, `KN`, `KP`, `KR`, `KW`, `KY`, `KZ`, `LA`, `LB`, `LC`, `LI`, `LK`, `LR`, `LS`, `LT`, `LU`, `LV`, `LY`, `MA`, `MC`, `MD`, `ME`, `MF`, `MG`, `MH`, `MK`, `ML`, `MM`, `MN`, `MO`, `MP`, `MQ`, `MR`, `MS`, `MT`, `MU`, `MV`, `MW`, `MX`, `MY`, `MZ`, `NA`, `NC`, `NE`, `NF`, `NG`, `NI`, `NL`, `NO`, `NP`, `NR`, `NU`, `NZ`, `OM`, `PA`, `PE`, `PF`, `PG`, `PH`, `PK`, `PL`, `PM`, `PN` |
| `countryOfManufacture.refName` | Reference Name | string |  |  |  |  |
| `createExpensePlansOn` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `createRevenuePlansOn` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `defaultItemShipMethod` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
| `deferRevRec` | Hold Revenue Recognition | boolean |  |  |  |  |
| `deferralAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `deferredRevenueAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `directRevenuePosting` | Direct Revenue Posting | boolean |  |  |  |  |
| `displayName` | Display Name/Code | string |  |  |  |  |
| `dontShowPrice` | Don't Show Price | boolean |  |  |  |  |
| `enforceminqtyinternally` | Enforce Minimum Internally | boolean |  |  |  |  |
| `excludeFromSiteMap` | Exclude from Sitemap | boolean |  |  |  |  |
| `expenseAmortizationRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `featuredDescription` | Featured Description | string |  |  |  |  |
| `froogleProductFeed` | Google Base Product Feed | boolean |  |  |  |  |
| `handlingCost` | Handling Cost | number | double |  |  |  |
| `hazmatHazardClass` | Hazmat Hazard Class | string |  |  |  |  |
| `hazmatId` | Hazmat Id | string |  |  |  |  |
| `hazmatItemUnits` | Hazmat Item Units | string |  |  |  |  |
| `hazmatItemUnitsQty` | Hazmat Item Units Quantity | number | float |  |  |  |
| `hazmatPackingGroup` |  | object |  |  |  |  |
| `hazmatPackingGroup.id` | Internal identifier | string |  |  |  | `DEFAULT`, `I`, `II`, `III` |
| `hazmatPackingGroup.refName` | Reference Name | string |  |  |  |  |
| `hazmatShippingName` | Hazmat Shipping Name | string |  |  |  |  |
| `hazmatTechnicalName` | Hazmat Technical Name | string |  |  |  |  |
| `hierarchyVersions` |  | nonInventorySaleItem-hierarchyVersionsCollection |  |  | [`nonInventorySaleItem-hierarchyVersionsCollection`](#noninventorysaleitem-hierarchyversionscollection) |  |
| `id` | Internal ID | string |  |  |  |  |
| `includeChildren` | Include Children | boolean |  |  |  |  |
| `incomeAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `insertItemAttribute` |  | object |  |  |  |  |
| `insertItemAttribute.id` | Internal identifier | string |  |  |  | `class`, `department`, `location`, `itemid`, `issueproduct`, `vendorname` |
| `insertItemAttribute.refName` | Reference Name | string |  |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `isDonationItem` | Variable Amount | boolean |  |  |  |  |
| `isFulfillable` | Can be Fulfilled | boolean |  |  |  |  |
| `isGCoCompliant` | Google Checkout Compliant | boolean |  |  |  |  |
| `isHazmatItem` | Hazmat/Dangerous Goods | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isOnline` | Display in Website | boolean |  |  |  |  |
| `isTaxable` | Taxable | boolean |  |  |  |  |
| `issueProduct` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `itemCarrier` |  | object |  |  |  |  |
| `itemCarrier.id` | Internal identifier | string |  |  |  | `ups`, `nonups` |
| `itemCarrier.refName` | Reference Name | string |  |  |  |  |
| `itemId` | Item Name/Number | string |  |  |  |  |
| `itemOptions` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `itemRevenueCategory` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `itemShipMethod` |  | shipItemCollection |  |  | [`shipItemCollection`](shipItem.md#shipitemcollection) |  |
| `itemType` |  | object |  |  |  |  |
| `itemType.id` | Internal identifier | string |  |  |  | `Group`, `Description`, `Discount`, `EndGroup`, `GiftCert`, `Subtotal`, `Service`, `ShipItem`, `TaxItem`, `InvtPart`, `Payment`, `Expense`, `NonInvtPart`, `TaxGroup`, `Kit`, `Markup`, `DwnLdItem`, `OthCharge`, `Assembly`, `SubscriPlan` |
| `itemType.refName` | Reference Name | string |  |  |  |  |
| `lastModifiedDate` | Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `manufacturer` | Manufacturer | string |  |  |  |  |
| `manufacturerAddr1` | Manufacturer Address | string |  |  |  |  |
| `manufacturerCity` | Manufacturer City | string |  |  |  |  |
| `manufacturerState` | Manufacturer State | string |  |  |  |  |
| `manufacturerTariff` | HS Tariff Number | string |  |  |  |  |
| `manufacturerTaxId` | Manufacturer Tax Id | string |  |  |  |  |
| `manufacturerZip` | Manufacturer Zip Code | string |  |  |  |  |
| `matrixItemNameTemplate` | Matrix Item Name Template | string |  |  |  |  |
| `matrixItemNameTemplateHelp` | Matrix Item Name Template | string |  |  |  |  |
| `matrixType` |  | object |  |  |  |  |
| `matrixType.id` | Internal identifier | string |  |  |  | `PARENT`, `CHILD` |
| `matrixType.refName` | Reference Name | string |  |  |  |  |
| `maxDonationAmount` | Maximum Variable Amount | number | double |  |  |  |
| `maximumquantity` | Maximum Order Qty | integer | int64 |  |  |  |
| `metaTagHtml` | Meta Tag HTML | string |  |  |  |  |
| `minimumquantity` | Minimum Order Qty | integer | int64 |  |  |  |
| `mpn` | Manufacturer Part Number | string |  |  |  |  |
| `multManufactureAddr` | Multiple Manufacturer Addresses | boolean |  |  |  |  |
| `nexTagCategory` | NexTag Category | string |  |  |  |  |
| `nexTagProductFeed` | NexTag Product Feed | boolean |  |  |  |  |
| `noPriceMessage` | No Price Message | string |  |  |  |  |
| `offerSupport` | Offer Support | boolean |  |  |  |  |
| `onSpecial` | On Special | boolean |  |  |  |  |
| `outOfStockBehavior` |  | object |  |  |  |  |
| `outOfStockBehavior.id` | Internal identifier | string |  |  |  | `DISABLE`, `ENABLENMSG`, `REMOVE`, `ENABLE`, `DEFAULT` |
| `outOfStockBehavior.refName` | Reference Name | string |  |  |  |  |
| `outOfStockMessage` | Out Of Stock Message | string |  |  |  |  |
| `overallQuantityPricingType` |  | object |  |  |  |  |
| `overallQuantityPricingType.id` | Internal identifier | string |  |  |  | `ITEM`, `PARENT`, `SCHEDULE` |
| `overallQuantityPricingType.refName` | Reference Name | string |  |  |  |  |
| `pageTitle` | Page Title | string |  |  |  |  |
| `parent` |  | nonInventorySaleItem |  |  | [`nonInventorySaleItem`](#noninventorysaleitem) |  |
| `parentOnly` | Use as Category Only | boolean |  |  |  |  |
| `preferenceCriterion` |  | object |  |  |  |  |
| `preferenceCriterion.id` | Internal identifier | string |  |  |  | `A`, `B`, `C`, `D`, `E`, `F` |
| `preferenceCriterion.refName` | Reference Name | string |  |  |  |  |
| `presentationItem` |  | nonInventorySaleItem-presentationItemCollection |  |  | [`nonInventorySaleItem-presentationItemCollection`](#noninventorysaleitem-presentationitemcollection) |  |
| `price` |  | nonInventorySaleItem-price |  |  | [`nonInventorySaleItem-price`](#noninventorysaleitem-price) |  |
| `pricesIncludeTax` | Prices Include Tax | boolean |  |  |  |  |
| `pricingGroup` |  | pricingGroup |  |  | [`pricingGroup`](pricingGroup.md#pricinggroup) |  |
| `producer` | Producer | boolean |  |  |  |  |
| `quantityPricingSchedule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `rate` | Price | number | double |  |  |  |
| `rateIncludingTax` | Price Including Tax | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `relatedItemsDescription` | Related Items Description | string |  |  |  |  |
| `residual` | Residual | number | double |  |  |  |
| `revRecForecastRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `revRecSchedule` |  | revRecTemplate |  |  | [`revRecTemplate`](revRecTemplate.md#revrectemplate) |  |
| `revReclassFxAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `revenueAllocationGroup` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `revenueRecognitionRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `saleUnit` | Primary Sale Unit | string |  |  |  |  |
| `salesDescription` | Sales Description | string |  |  |  |  |
| `salesTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `scheduleBCode` |  | object |  |  |  |  |
| `scheduleBCode.id` | Internal identifier | string |  |  |  | `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `10`, `32`, `11`, `33`, `12`, `13`, `14`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21` |
| `scheduleBCode.refName` | Reference Name | string |  |  |  |  |
| `scheduleBNumber` | Schedule B Number | string |  |  |  |  |
| `scheduleBQuantity` | Schedule B Quantity | number | float |  |  |  |
| `searchKeywords` | Search Keywords | string |  |  |  |  |
| `shipIndividually` | Ships Individually | boolean |  |  |  |  |
| `shipPackage` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `shippingCost` | Shipping Cost | number | double |  |  |  |
| `shoppingDotComCategory` | Shopping.com Category | string |  |  |  |  |
| `shoppingProductFeed` | Shopping Product Feed | boolean |  |  |  |  |
| `shopzillaCategoryId` | Shopzilla Category ID | integer | int64 |  |  |  |
| `shopzillaProductFeed` | Shopzilla Product Feed | boolean |  |  |  |  |
| `showDefaultDonationAmount` | Show Default Amount | boolean |  |  |  |  |
| `siteCategory` |  | nonInventorySaleItem-siteCategoryCollection |  |  | [`nonInventorySaleItem-siteCategoryCollection`](#noninventorysaleitem-sitecategorycollection) |  |
| `siteMapPriority` |  | object |  |  |  |  |
| `siteMapPriority.id` | Internal identifier | string |  |  |  | `0.0`, `0.1`, `0.2`, `0.3`, `0.4`, `0.5`, `0.6`, `0.7`, `0.8`, `0.9`, `1.0` |
| `siteMapPriority.refName` | Reference Name | string |  |  |  |  |
| `softDescriptor` |  | object |  |  |  |  |
| `softDescriptor.id` | Internal identifier | string |  |  |  | `1`, `2` |
| `softDescriptor.refName` | Reference Name | string |  |  |  |  |
| `stockDescription` | Stock Description | string |  |  |  |  |
| `storeDescription` | Store Description | string |  |  |  |  |
| `storeDetailedDescription` | Detailed Description | string |  |  |  |  |
| `storeDisplayImage` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `storeDisplayName` | Store Display Name | string |  |  |  |  |
| `storeDisplayThumbnail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `storeItemTemplate` |  | object |  |  |  |  |
| `storeItemTemplate.id` | Internal identifier | string |  |  |  | `-134`, `-178`, `-133`, `-177`, `-136`, `-179`, `-135`, `-130`, `-174`, `-173`, `-176`, `-132`, `-131`, `-175`, `-138`, `-137`, `-139`, `-150`, `-101`, `-145`, `-144`, `-100`, `-103`, `-147`, `-102`, `-146`, `-141`, `-140`, `-143`, `-142`, `-109`, `-108`, `-149`, `-105`, `-148`, `-104`, `-107`, `-106`, `-161`, `-160`, `-156`, `-112`, `-111`, `-155`, `-158`, `-114`, `-157`, `-113`, `-110`, `-154`, `-153`, `-119`, `-116`, `-159`, `-115`, `-118`, `-117`, `-170`, `-172`, `-171`, `-123`, `-122`, `-125`, `-124`, `-162`, `-121`, `-120`, `-127`, `-126`, `-129`, `-128` |
| `storeItemTemplate.refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiaryCollection |  |  | [`subsidiaryCollection`](subsidiary.md#subsidiarycollection) |  |
| `taxSchedule` |  | taxSchedule |  |  | [`taxSchedule`](taxSchedule.md#taxschedule) |  |
| `tracksaasmetrics` | SaaS Metric Tracking | boolean |  |  |  |  |
| `tracksaasmetricsenddate` | SaaS Metric End Date | string | date |  |  |  |
| `tracksaasmetricsstartdate` | SaaS Metric Start Date | string | date |  |  |  |
| `translations` |  | nonInventorySaleItem-translationsCollection |  |  | [`nonInventorySaleItem-translationsCollection`](#noninventorysaleitem-translationscollection) |  |
| `unitsType` |  | unitsType |  |  | [`unitsType`](unitsType.md#unitstype) |  |
| `upcCode` | UPC Code | string |  |  |  |  |
| `urlComponent` | URL Component | string |  |  |  |  |
| `useMarginalRates` | Use Marginal Rates | boolean |  |  |  |  |
| `weight` | Item Weight | number | float |  |  |  |
| `weightUnit` |  | object |  |  |  |  |
| `weightUnit.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `weightUnit.refName` | Reference Name | string |  |  |  |  |
| `weightUnits` | Weight Units | string |  |  |  |  |
| `yahooProductFeed` | Yahoo Shopping Product Feed | boolean |  |  |  |  |

## nonInventorySaleItem-accountingBookDetailCollection

Browser definition `nonInventorySaleItem-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | nonInventorySaleItem-accountingBookDetailElement[] |  |  | [`nonInventorySaleItem-accountingBookDetailElement`](#noninventorysaleitem-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nonInventorySaleItem-accountingBookDetailElement

Browser definition `nonInventorySaleItem-accountingBookDetailElement`.

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

## nonInventorySaleItem-correlatedItemsCollection

Browser definition `nonInventorySaleItem-correlatedItemsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | nonInventorySaleItem-correlatedItemsElement[] |  |  | [`nonInventorySaleItem-correlatedItemsElement`](#noninventorysaleitem-correlateditemselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nonInventorySaleItem-correlatedItemsElement

Browser definition `nonInventorySaleItem-correlatedItemsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `correlationFld` | Correlation % | number | double |  |  |  |
| `countFld` | Count | integer | int64 |  |  |  |
| `itemNKeyFld` | Item | string |  |  |  |  |
| `liftFld` | Lift % | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `purchaseRateFld` | Overall Purchase Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## nonInventorySaleItem-hierarchyVersionsCollection

Browser definition `nonInventorySaleItem-hierarchyVersionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | nonInventorySaleItem-hierarchyVersionsElement[] |  |  | [`nonInventorySaleItem-hierarchyVersionsElement`](#noninventorysaleitem-hierarchyversionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nonInventorySaleItem-hierarchyVersionsElement

Browser definition `nonInventorySaleItem-hierarchyVersionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `endDate` | Hierarchy Version End Date | string | date |  |  |  |
| `hierarchyNode` |  | merchandiseHierarchyNode |  |  | [`merchandiseHierarchyNode`](merchandiseHierarchyNode.md#merchandisehierarchynode) |  |
| `hierarchyVersion` |  | merchandiseHierarchyVersion |  |  | [`merchandiseHierarchyVersion`](merchandiseHierarchyVersion.md#merchandisehierarchyversion) |  |
| `isIncluded` | Included In Version | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `startDate` | Hierarchy Version Start Date | string | date |  |  |  |

## nonInventorySaleItem-presentationItemCollection

Browser definition `nonInventorySaleItem-presentationItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | nonInventorySaleItem-presentationItemElement[] |  |  | [`nonInventorySaleItem-presentationItemElement`](#noninventorysaleitem-presentationitemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nonInventorySaleItem-presentationItemElement

Browser definition `nonInventorySaleItem-presentationItemElement`.

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

## nonInventorySaleItem-price

Browser definition `nonInventorySaleItem-price`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | nonInventorySaleItem-priceElement[] |  |  | [`nonInventorySaleItem-priceElement`](#noninventorysaleitem-priceelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nonInventorySaleItem-priceElement

Browser definition `nonInventorySaleItem-priceElement`.

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

## nonInventorySaleItem-siteCategoryCollection

Browser definition `nonInventorySaleItem-siteCategoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | nonInventorySaleItem-siteCategoryElement[] |  |  | [`nonInventorySaleItem-siteCategoryElement`](#noninventorysaleitem-sitecategoryelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nonInventorySaleItem-siteCategoryElement

Browser definition `nonInventorySaleItem-siteCategoryElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `category` |  | siteCategory |  |  | [`siteCategory`](siteCategory.md#sitecategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `webSite` |  | webSite |  |  | [`webSite`](webSite.md#website) |  |

## nonInventorySaleItem-translationsCollection

Browser definition `nonInventorySaleItem-translationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | nonInventorySaleItem-translationsElement[] |  |  | [`nonInventorySaleItem-translationsElement`](#noninventorysaleitem-translationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nonInventorySaleItem-translationsElement

Browser definition `nonInventorySaleItem-translationsElement`.

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

## nonInventorySaleItemCollection

Browser definition `nonInventorySaleItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | nonInventorySaleItem[] |  |  | [`nonInventorySaleItem`](#noninventorysaleitem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## nonInventorySaleItemSelectOptions

Browser definition `nonInventorySaleItemSelectOptions`.

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
| `countryOfManufacture` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createExpensePlansOn` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createRevenuePlansOn` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultItemShipMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deferralAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deferredRevenueAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `expenseAmortizationRule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `hazmatPackingGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `incomeAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `insertItemAttribute` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `issueProduct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemCarrier` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemOptions` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemRevenueCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemShipMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `matrixType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `outOfStockBehavior` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `overallQuantityPricingType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `preferenceCriterion` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `pricingGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `quantityPricingSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revRecForecastRule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revRecSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revReclassFxAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revenueAllocationGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revenueRecognitionRule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `saleUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `scheduleBCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipPackage` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `siteMapPriority` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `softDescriptor` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `storeDisplayImage` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `storeDisplayThumbnail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `storeItemTemplate` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `unitsType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `weightUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

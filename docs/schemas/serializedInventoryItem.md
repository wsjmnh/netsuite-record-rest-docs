# Schemas: serializedInventoryItem

Property tables for definitions owned by `serializedInventoryItem`.

Record page: [serializedInventoryItem](../records/serializedInventoryItem.md).

## Index

- [serializedInventoryItem](#serializedinventoryitem) — 333 properties
- [serializedInventoryItem-accountingBookDetailCollection](#serializedinventoryitem-accountingbookdetailcollection) — 6 properties
- [serializedInventoryItem-accountingBookDetailElement](#serializedinventoryitem-accountingbookdetailelement) — 11 properties
- [serializedInventoryItem-binNumberCollection](#serializedinventoryitem-binnumbercollection) — 6 properties
- [serializedInventoryItem-binNumberElement](#serializedinventoryitem-binnumberelement) — 9 properties
- [serializedInventoryItem-consignedlocationsCollection](#serializedinventoryitem-consignedlocationscollection) — 6 properties
- [serializedInventoryItem-consignedlocationsElement](#serializedinventoryitem-consignedlocationselement) — 11 properties
- [serializedInventoryItem-correlatedItemsCollection](#serializedinventoryitem-correlateditemscollection) — 6 properties
- [serializedInventoryItem-correlatedItemsElement](#serializedinventoryitem-correlateditemselement) — 7 properties
- [serializedInventoryItem-hierarchyVersionsCollection](#serializedinventoryitem-hierarchyversionscollection) — 6 properties
- [serializedInventoryItem-hierarchyVersionsElement](#serializedinventoryitem-hierarchyversionselement) — 7 properties
- [serializedInventoryItem-itemVendor-itemVendorPrice](#serializedinventoryitem-itemvendor-itemvendorprice) — 4 properties
- [serializedInventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection](#serializedinventoryitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) — 6 properties
- [serializedInventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement](#serializedinventoryitem-itemvendor-itemvendorprice-itemvendorpricelineselement) — 6 properties
- [serializedInventoryItem-itemVendorCollection](#serializedinventoryitem-itemvendorcollection) — 6 properties
- [serializedInventoryItem-itemVendorElement](#serializedinventoryitem-itemvendorelement) — 13 properties
- [serializedInventoryItem-locationsCollection](#serializedinventoryitem-locationscollection) — 6 properties
- [serializedInventoryItem-locationsElement](#serializedinventoryitem-locationselement) — 72 properties
- [serializedInventoryItem-numbersCollection](#serializedinventoryitem-numberscollection) — 6 properties
- [serializedInventoryItem-numbersElement](#serializedinventoryitem-numberselement) — 7 properties
- [serializedInventoryItem-presentationItemCollection](#serializedinventoryitem-presentationitemcollection) — 6 properties
- [serializedInventoryItem-presentationItemElement](#serializedinventoryitem-presentationitemelement) — 11 properties
- [serializedInventoryItem-price](#serializedinventoryitem-price) — 6 properties
- [serializedInventoryItem-priceElement](#serializedinventoryitem-priceelement) — 10 properties
- [serializedInventoryItem-siteCategoryCollection](#serializedinventoryitem-sitecategorycollection) — 6 properties
- [serializedInventoryItem-siteCategoryElement](#serializedinventoryitem-sitecategoryelement) — 4 properties
- [serializedInventoryItem-translationsCollection](#serializedinventoryitem-translationscollection) — 6 properties
- [serializedInventoryItem-translationsElement](#serializedinventoryitem-translationselement) — 16 properties
- [serializedInventoryItemCollection](#serializedinventoryitemcollection) — 6 properties
- [serializedInventoryItemSelectOptions](#serializedinventoryitemselectoptions) — 98 properties

## serializedInventoryItem

Browser definition `serializedInventoryItem`.

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
| `accountingBookDetail` |  | serializedInventoryItem-accountingBookDetailCollection |  |  | [`serializedInventoryItem-accountingBookDetailCollection`](#serializedinventoryitem-accountingbookdetailcollection) |  |
| `allowconsignment` | Allow Vendor Consignment | boolean |  |  |  |  |
| `alternateDemandSourceItem` |  | serializedInventoryItem |  |  | [`serializedInventoryItem`](#serializedinventoryitem) |  |
| `amortizationPeriod` | Amortization Period | integer | int64 |  |  |  |
| `amortizationTemplate` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `assetAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `atpLeadTime` | ATP Lead Time | integer | int64 |  |  |  |
| `atpMethod` |  | object |  |  |  |  |
| `atpMethod.id` | Internal identifier | string |  |  |  | `CUMULATIVE_ATP_WITH_LOOK_AHEAD`, `DISCRETE_ATP` |
| `atpMethod.refName` | Reference Name | string |  |  |  |  |
| `autoExpandKitForRevenuemgmt` | Auto-Expansion for Revenue Management | boolean |  |  |  |  |
| `autoLeadTime` | Auto-Calculate Lead Time | boolean |  |  |  |  |
| `autoPreferredStockLevel` | Auto-Calculate Preferred Stock Level | boolean |  |  |  |  |
| `autoReorderPoint` | Auto-Calculate Reorder Point | boolean |  |  |  |  |
| `availableToPartners` | Available to Adv. Partners | boolean |  |  |  |  |
| `averageCost` | Average Cost | number | double |  |  |  |
| `backwardConsumptionDays` | Backward Consumption Days | integer | int64 |  |  |  |
| `baseUnit` | Primary Base Unit | string |  |  |  |  |
| `billExchRateVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `billPriceVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `billQtyVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `billingSchedule` |  | billingSchedule |  |  | [`billingSchedule`](billingSchedule.md#billingschedule) |  |
| `binNumber` |  | serializedInventoryItem-binNumberCollection |  |  | [`serializedInventoryItem-binNumberCollection`](#serializedinventoryitem-binnumbercollection) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `cogsAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `consignedlocations` |  | serializedInventoryItem-consignedlocationsCollection |  |  | [`serializedInventoryItem-consignedlocationsCollection`](#serializedinventoryitem-consignedlocationscollection) |  |
| `consignmentassetaccount` |  | account |  |  | [`account`](account.md#account) |  |
| `consignmentexpenseaccount` |  | account |  |  | [`account`](account.md#account) |  |
| `consumptionUnit` | Primary Consumption Unit | string |  |  |  |  |
| `contingentRevenueHandling` | Eligible For Contingent Revenue Handling | boolean |  |  |  |  |
| `conversionRate` | Conversion Rate (/Primary Base) | number | float |  |  |  |
| `copyDescription` | Copy from Sales Order | boolean |  |  |  |  |
| `correlatedItems` |  | serializedInventoryItem-correlatedItemsCollection |  |  | [`serializedInventoryItem-correlatedItemsCollection`](#serializedinventoryitem-correlateditemscollection) |  |
| `cost` | Purchase Price | number | double |  |  |  |
| `costAccountingStatus` | Cost Accounting Status | string |  |  |  |  |
| `costCategory` |  | costCategory |  |  | [`costCategory`](costCategory.md#costcategory) |  |
| `costEstimate` | Item Defined Cost | number | double |  |  |  |
| `costEstimateUnits` | Est. Cost Unit | string |  |  |  |  |
| `costForPricing` | Cost for Pricing | number | double |  |  |  |
| `costingMethod` |  | object |  |  |  |  |
| `costingMethod.id` | Internal identifier | string |  |  |  | `SERIAL`, `LOT`, `AVG`, `LIFO`, `GROUPAVG`, `FIFO`, `STANDARD` |
| `costingMethod.refName` | Reference Name | string |  |  |  |  |
| `countryOfManufacture` |  | object |  |  |  |  |
| `countryOfManufacture.id` | Internal identifier | string |  |  |  | `PR`, `PS`, `PT`, `PW`, `PY`, `QA`, `AB`, `AD`, `AE`, `AF`, `AG`, `AI`, `AL`, `AM`, `AN`, `AO`, `AQ`, `AR`, `AS`, `AT`, `RE`, `AU`, `AW`, `AX`, `AZ`, `RO`, `BA`, `BB`, `RS`, `BD`, `BE`, `RU`, `BF`, `BG`, `RW`, `BH`, `BI`, `BJ`, `BL`, `BM`, `BN`, `BO`, `SA`, `BQ`, `SB`, `BR`, `SC`, `BS`, `SD`, `BT`, `SE`, `BV`, `SG`, `BW`, `SH`, `SI`, `BY`, `SJ`, `BZ`, `SK`, `SL`, `SM`, `SN`, `SO`, `CA`, `SR`, `CC`, `SS`, `CD`, `ST`, `CF`, `SV`, `CG`, `CH`, `SX`, `CI`, `SY`, `SZ`, `CK`, `CL`, `CM`, `CN`, `CO`, `CR`, `TC`, `CS`, `TD`, `CU`, `TF`, `CV`, `TG`, `CW`, `TH`, `CX`, `CY`, `TJ`, `CZ`, `TK`, `TL`, `TM`, `TN`, `TO`, `TR`, `TT`, `DE`, `TV`, `TW`, `DJ`, `TZ`, `DK`, `DM`, `DO`, `UA`, `UG`, `DZ`, `UM`, `EA`, `EC`, `US`, `EE`, `EG`, `EH`, `UY`, `UZ`, `VA`, `ER`, `VC`, `ES`, `ET`, `VE`, `VG`, `VI`, `VN`, `VU`, `FI`, `FJ`, `FK`, `FM`, `FO`, `FR`, `WF`, `GA`, `GB`, `WS`, `GD`, `GE`, `GF`, `GG`, `GH`, `GI`, `GL`, `GM`, `GN`, `GP`, `GQ`, `GR`, `GS`, `GT`, `GU`, `GW`, `GY`, `XK`, `HK`, `HM`, `HN`, `HR`, `HT`, `YE`, `HU`, `IC`, `ID`, `YT`, `IE`, `IL`, `IM`, `IN`, `IO`, `ZA`, `IQ`, `IR`, `IS`, `IT`, `ZM`, `JE`, `ZW`, `JM`, `JO`, `JP`, `KE`, `KG`, `KH`, `KI`, `KM`, `KN`, `KP`, `KR`, `KW`, `KY`, `KZ`, `LA`, `LB`, `LC`, `LI`, `LK`, `LR`, `LS`, `LT`, `LU`, `LV`, `LY`, `MA`, `MC`, `MD`, `ME`, `MF`, `MG`, `MH`, `MK`, `ML`, `MM`, `MN`, `MO`, `MP`, `MQ`, `MR`, `MS`, `MT`, `MU`, `MV`, `MW`, `MX`, `MY`, `MZ`, `NA`, `NC`, `NE`, `NF`, `NG`, `NI`, `NL`, `NO`, `NP`, `NR`, `NU`, `NZ`, `OM`, `PA`, `PE`, `PF`, `PG`, `PH`, `PK`, `PL`, `PM`, `PN` |
| `countryOfManufacture.refName` | Reference Name | string |  |  |  |  |
| `createExpensePlansOn` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `createRevenuePlansOn` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `custReturnVarianceAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `dateConvertedToInv` | Date Converted To Inv. | string | date-time |  |  |  |
| `defaultAllocationStrategy` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `defaultItemShipMethod` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
| `defaultReturnCost` | Default Return Cost | number | double |  |  |  |
| `defaultReturnCostUnits` |  | string |  |  |  |  |
| `deferRevRec` | Hold Revenue Recognition | boolean |  |  |  |  |
| `deferralAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `deferredRevenueAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `demandModifier` | Estimated Demand Change | number | double |  |  |  |
| `demandSource` |  | object |  |  |  |  |
| `demandSource.id` | Internal identifier | string |  |  |  | `FORECASTANDORDERS`, `EXISTINGORDERSANDDEPENDENTDEMAND`, `FORECASTCONSUMPTION`, `ITEMDEMANDPLAN` |
| `demandSource.refName` | Reference Name | string |  |  |  |  |
| `demandTimeFence` | Demand Time Fence | integer | int64 |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `directRevenuePosting` | Direct Revenue Posting | boolean |  |  |  |  |
| `displayName` | Display Name/Code | string |  |  |  |  |
| `distributionCategory` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `distributionNetwork` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `dontShowPrice` | Don't Show Price | boolean |  |  |  |  |
| `dropShipExpenseAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `enableCatchWeight` | Enable Catch Weight | boolean |  |  |  |  |
| `enforceminqtyinternally` | Enforce Minimum Internally | boolean |  |  |  |  |
| `excludeFromSiteMap` | Exclude from Sitemap | boolean |  |  |  |  |
| `expenseAmortizationRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `featuredDescription` | Featured Description | string |  |  |  |  |
| `fixedLotSize` | Fixed Lot Size | number | float |  |  |  |
| `fixedLotSizeUnits` |  | string |  |  |  |  |
| `forwardConsumptionDays` | Forward Consumption Days | integer | int64 |  |  |  |
| `fraudRisk` |  | object |  |  |  |  |
| `fraudRisk.id` | Internal identifier | string |  |  |  | `LOW`, `MEDIUM`, `HIGH` |
| `fraudRisk.refName` | Reference Name | string |  |  |  |  |
| `froogleProductFeed` | Google Base Product Feed | boolean |  |  |  |  |
| `futurehorizon` | Supply Chain Future Horizon | integer | int64 |  |  |  |
| `gainLossAccount` |  | account |  |  | [`account`](account.md#account) |  |
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
| `hierarchyVersions` |  | serializedInventoryItem-hierarchyVersionsCollection |  |  | [`serializedInventoryItem-hierarchyVersionsCollection`](#serializedinventoryitem-hierarchyversionscollection) |  |
| `id` | Internal ID | string |  |  |  |  |
| `includeChildren` | Include Children | boolean |  |  |  |  |
| `incomeAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `insertItemAttribute` |  | object |  |  |  |  |
| `insertItemAttribute.id` | Internal identifier | string |  |  |  | `class`, `department`, `location`, `itemid`, `issueproduct`, `vendorname` |
| `insertItemAttribute.refName` | Reference Name | string |  |  |  |  |
| `interCoDefRevAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `intercoCogsAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `intercoExpenseAccountHidden` |  | string |  |  |  |  |
| `intercoIncomeAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `invtClassification` |  | object |  |  |  |  |
| `invtClassification.id` | Internal identifier | string |  |  |  | `1`, `2`, `3` |
| `invtClassification.refName` | Reference Name | string |  |  |  |  |
| `invtCountInterval` | Count Interval | integer | int64 |  |  |  |
| `isDonationItem` | Variable Amount | boolean |  |  |  |  |
| `isDropShipItem` | Drop Ship Item | boolean |  |  |  |  |
| `isGCoCompliant` | Google Checkout Compliant | boolean |  |  |  |  |
| `isHazmatItem` | Hazmat/Dangerous Goods | boolean |  |  |  |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isLotItem` | Lot Numbered | boolean |  |  |  |  |
| `isOnline` | Display in Website | boolean |  |  |  |  |
| `isSerialItem` | Serialized | boolean |  |  |  |  |
| `isSpecialOrderItem` | Special Order Item | boolean |  |  |  |  |
| `isStorePickupAllowed` | Store Pickup Allowed | boolean |  |  |  |  |
| `isTaxable` | Taxable | boolean |  |  |  |  |
| `issueProduct` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `itemCarrier` |  | object |  |  |  |  |
| `itemCarrier.id` | Internal identifier | string |  |  |  | `ups`, `nonups` |
| `itemCarrier.refName` | Reference Name | string |  |  |  |  |
| `itemId` | Item Name/Number | string |  |  |  |  |
| `itemOptions` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `itemProcessFamily` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `itemProcessGroup` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `itemRevenueCategory` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `itemShipMethod` |  | shipItemCollection |  |  | [`shipItemCollection`](shipItem.md#shipitemcollection) |  |
| `itemType` |  | object |  |  |  |  |
| `itemType.id` | Internal identifier | string |  |  |  | `Group`, `Description`, `Discount`, `EndGroup`, `GiftCert`, `Subtotal`, `Service`, `ShipItem`, `TaxItem`, `InvtPart`, `Payment`, `Expense`, `NonInvtPart`, `TaxGroup`, `Kit`, `Markup`, `DwnLdItem`, `OthCharge`, `Assembly`, `SubscriPlan` |
| `itemType.refName` | Reference Name | string |  |  |  |  |
| `itemVendor` |  | serializedInventoryItem-itemVendorCollection |  |  | [`serializedInventoryItem-itemVendorCollection`](#serializedinventoryitem-itemvendorcollection) |  |
| `lastInvtCountDate` | Last Count Date | string | date |  |  |  |
| `lastModifiedDate` | Last Modified | string | date-time |  |  |  |
| `lastPurchasePrice` | Last Purchase Price | number | double |  |  |  |
| `leadTime` | Purchase Lead Time | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `locations` |  | serializedInventoryItem-locationsCollection |  |  | [`serializedInventoryItem-locationsCollection`](#serializedinventoryitem-locationscollection) |  |
| `lowerWarningLimit` | Lower Warning Limit % (-) | number | float |  |  |  |
| `manufacturer` | Manufacturer | string |  |  |  |  |
| `manufacturerAddr1` | Manufacturer Address | string |  |  |  |  |
| `manufacturerCity` | Manufacturer City | string |  |  |  |  |
| `manufacturerState` | Manufacturer State | string |  |  |  |  |
| `manufacturerTariff` | HS Tariff Number | string |  |  |  |  |
| `manufacturerTaxId` | Manufacturer Tax Id | string |  |  |  |  |
| `manufacturerZip` | Manufacturer Zip Code | string |  |  |  |  |
| `matchBillToReceipt` | Match Bill To Receipt | boolean |  |  |  |  |
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
| `nextInvtCountDate` | Next Count Date | string | date |  |  |  |
| `noPriceMessage` | No Price Message | string |  |  |  |  |
| `numbers` |  | serializedInventoryItem-numbersCollection |  |  | [`serializedInventoryItem-numbersCollection`](#serializedinventoryitem-numberscollection) |  |
| `offerSupport` | Offer Support | boolean |  |  |  |  |
| `onSpecial` | On Special | boolean |  |  |  |  |
| `originalItemSubtype` | Original Item Subtype | string |  |  |  |  |
| `originalItemType` | Original Item Type | string |  |  |  |  |
| `outOfStockBehavior` |  | object |  |  |  |  |
| `outOfStockBehavior.id` | Internal identifier | string |  |  |  | `DISABLE`, `ENABLENMSG`, `REMOVE`, `ENABLE`, `DEFAULT` |
| `outOfStockBehavior.refName` | Reference Name | string |  |  |  |  |
| `outOfStockMessage` | Out Of Stock Message | string |  |  |  |  |
| `overallQuantityPricingType` |  | object |  |  |  |  |
| `overallQuantityPricingType.id` | Internal identifier | string |  |  |  | `ITEM`, `PARENT`, `SCHEDULE` |
| `overallQuantityPricingType.refName` | Reference Name | string |  |  |  |  |
| `pageTitle` | Page Title | string |  |  |  |  |
| `parent` |  | serializedInventoryItem |  |  | [`serializedInventoryItem`](#serializedinventoryitem) |  |
| `parentOnly` | Use as Category Only | boolean |  |  |  |  |
| `periodicLotSizeDays` | Periods of Supply Increment | integer | int64 |  |  |  |
| `periodicLotSizeType` |  | object |  |  |  |  |
| `periodicLotSizeType.id` | Internal identifier | string |  |  |  | `INTERVAL`, `WEEKLY`, `MONTHLY` |
| `periodicLotSizeType.refName` | Reference Name | string |  |  |  |  |
| `planningItemCategory` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `preferenceCriterion` |  | object |  |  |  |  |
| `preferenceCriterion.id` | Internal identifier | string |  |  |  | `A`, `B`, `C`, `D`, `E`, `F` |
| `preferenceCriterion.refName` | Reference Name | string |  |  |  |  |
| `preferredLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `preferredStockLevel` | Preferred Stock Level | number | float |  |  |  |
| `preferredStockLevelDays` | Days | number | float |  |  |  |
| `preferredStockLevelUnits` |  | string |  |  |  |  |
| `presentationItem` |  | serializedInventoryItem-presentationItemCollection |  |  | [`serializedInventoryItem-presentationItemCollection`](#serializedinventoryitem-presentationitemcollection) |  |
| `price` |  | serializedInventoryItem-price |  |  | [`serializedInventoryItem-price`](#serializedinventoryitem-price) |  |
| `pricesIncludeTax` | Prices Include Tax | boolean |  |  |  |  |
| `pricingGroup` |  | pricingGroup |  |  | [`pricingGroup`](pricingGroup.md#pricinggroup) |  |
| `producer` | Producer | boolean |  |  |  |  |
| `purchaseDescription` | Purchase Description | string |  |  |  |  |
| `purchaseOrderAmount` | Vendor Bill - Purchase Order Amount Tolerance | number | float |  |  |  |
| `purchaseOrderQuantity` | Vendor Bill - Purchase Order Quantity Tolerance | number | float |  |  |  |
| `purchaseOrderQuantityDiff` | Vendor Bill - Purchase Order Quantity Difference | number | float |  |  |  |
| `purchasePriceVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `purchaseTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `purchaseUnit` | Primary Purchase Unit | string |  |  |  |  |
| `quantityAvailable` | Quantity Available | number | float |  |  |  |
| `quantityAvailableBase` | Quantity Available (Base Unit) | number | float |  |  |  |
| `quantityBackOrdered` | Quantity Back Ordered | number | float |  |  |  |
| `quantityCommitted` | Quantity Committed | number | float |  |  |  |
| `quantityOnHand` | Quantity On Hand | number | float |  |  |  |
| `quantityOnHandBase` | Quantity On Hand (Base Unit) | number | float |  |  |  |
| `quantityOnHandUnits` | Quantity On Hand Units | string |  |  |  |  |
| `quantityOnOrder` | Quantity On Order | number | float |  |  |  |
| `quantityPricingSchedule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `rate` | Price | number | double |  |  |  |
| `rateIncludingTax` | Price Including Tax | number | double |  |  |  |
| `receiptAmount` | Vendor Bill - Item Receipt Amount Tolerance | number | float |  |  |  |
| `receiptQuantity` | Vendor Bill - Item Receipt Quantity Tolerance | number | float |  |  |  |
| `receiptQuantityDiff` | Vendor Bill - Item Receipt Quantity Difference | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `relatedItemsDescription` | Related Items Description | string |  |  |  |  |
| `reorderMultiple` | Reorder Multiple | integer | int64 |  |  |  |
| `reorderPoint` | Reorder Point | number | float |  |  |  |
| `reorderPointUnits` |  | string |  |  |  |  |
| `rescheduleInDays` | Reschedule In Days | integer | int64 |  |  |  |
| `rescheduleOutDays` | Reschedule Out Days | integer | int64 |  |  |  |
| `residual` | Residual | number | double |  |  |  |
| `revRecForecastRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `revRecSchedule` |  | revRecTemplate |  |  | [`revRecTemplate`](revRecTemplate.md#revrectemplate) |  |
| `revReclassFxAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `revenueAllocationGroup` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `revenueRecognitionRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `rotationType` |  | object |  |  |  |  |
| `rotationType.id` | Internal identifier | string |  |  |  | `LEFO`, `FEFO` |
| `rotationType.refName` | Reference Name | string |  |  |  |  |
| `roundUpAsComponent` | Round Up Quantity as Component | boolean |  |  |  |  |
| `safetyStockLevel` | Safety Stock Level | number | float |  |  |  |
| `safetyStockLevelDays` | Safety Stock Level Days | integer | int64 |  |  |  |
| `saleUnit` | Primary Sale Unit | string |  |  |  |  |
| `salesDescription` | Sales Description | string |  |  |  |  |
| `salesTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `savedReorderPoint` | Reorder Point | number | float |  |  |  |
| `scheduleBCode` |  | object |  |  |  |  |
| `scheduleBCode.id` | Internal identifier | string |  |  |  | `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `10`, `32`, `11`, `33`, `12`, `13`, `14`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21` |
| `scheduleBCode.refName` | Reference Name | string |  |  |  |  |
| `scheduleBNumber` | Schedule B Number | string |  |  |  |  |
| `scheduleBQuantity` | Schedule B Quantity | number | float |  |  |  |
| `searchKeywords` | Search Keywords | string |  |  |  |  |
| `seasonalDemand` | Seasonal Demand | boolean |  |  |  |  |
| `secondaryBaseUnit` | Secondary Base Unit | string |  |  |  |  |
| `secondaryConsumptionUnit` | Secondary Consumption Unit | string |  |  |  |  |
| `secondaryPurchaseUnit` | Secondary Purchase Unit | string |  |  |  |  |
| `secondarySaleUnit` | Secondary Sale Unit | string |  |  |  |  |
| `secondaryStockUnit` | Secondary Stock Unit | string |  |  |  |  |
| `secondaryUnitsType` |  | unitsType |  |  | [`unitsType`](unitsType.md#unitstype) |  |
| `serialNumbers` | Serial Numbers | string |  |  |  |  |
| `shipIndividually` | Ships Individually | boolean |  |  |  |  |
| `shipPackage` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `shippingCost` | Shipping Cost | number | double |  |  |  |
| `shoppingDotComCategory` | Shopping.com Category | string |  |  |  |  |
| `shoppingProductFeed` | Shopping Product Feed | boolean |  |  |  |  |
| `shopzillaCategoryId` | Shopzilla Category ID | integer | int64 |  |  |  |
| `shopzillaProductFeed` | Shopzilla Product Feed | boolean |  |  |  |  |
| `showDefaultDonationAmount` | Show Default Amount | boolean |  |  |  |  |
| `siteCategory` |  | serializedInventoryItem-siteCategoryCollection |  |  | [`serializedInventoryItem-siteCategoryCollection`](#serializedinventoryitem-sitecategorycollection) |  |
| `siteMapPriority` |  | object |  |  |  |  |
| `siteMapPriority.id` | Internal identifier | string |  |  |  | `0.0`, `0.1`, `0.2`, `0.3`, `0.4`, `0.5`, `0.6`, `0.7`, `0.8`, `0.9`, `1.0` |
| `siteMapPriority.refName` | Reference Name | string |  |  |  |  |
| `softDescriptor` |  | object |  |  |  |  |
| `softDescriptor.id` | Internal identifier | string |  |  |  | `1`, `2` |
| `softDescriptor.refName` | Reference Name | string |  |  |  |  |
| `stockDescription` | Stock Description | string |  |  |  |  |
| `stockUnit` | Primary Stock Unit | string |  |  |  |  |
| `storeDescription` | Store Description | string |  |  |  |  |
| `storeDetailedDescription` | Detailed Description | string |  |  |  |  |
| `storeDisplayImage` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `storeDisplayName` | Store Display Name | string |  |  |  |  |
| `storeDisplayThumbnail` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `storeItemTemplate` |  | object |  |  |  |  |
| `storeItemTemplate.id` | Internal identifier | string |  |  |  | `-134`, `-178`, `-133`, `-177`, `-136`, `-179`, `-135`, `-130`, `-174`, `-173`, `-176`, `-132`, `-131`, `-175`, `-138`, `-137`, `-139`, `-150`, `-101`, `-145`, `-144`, `-100`, `-103`, `-147`, `-102`, `-146`, `-141`, `-140`, `-143`, `-142`, `-109`, `-108`, `-149`, `-105`, `-148`, `-104`, `-107`, `-106`, `-161`, `-160`, `-156`, `-112`, `-111`, `-155`, `-158`, `-114`, `-157`, `-113`, `-110`, `-154`, `-153`, `-119`, `-116`, `-159`, `-115`, `-118`, `-117`, `-170`, `-172`, `-171`, `-123`, `-122`, `-125`, `-124`, `-162`, `-121`, `-120`, `-127`, `-126`, `-129`, `-128` |
| `storeItemTemplate.refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiaryCollection |  |  | [`subsidiaryCollection`](subsidiary.md#subsidiarycollection) |  |
| `supplyLotSizingMethod` |  | object |  |  |  |  |
| `supplyLotSizingMethod.id` | Internal identifier | string |  |  |  | `FIXED_LOT_SIZE`, `LOT_FOR_LOT`, `FIXED_LOT_MULTIPLE`, `PERIODIC_LOT_SIZE` |
| `supplyLotSizingMethod.refName` | Reference Name | string |  |  |  |  |
| `supplyReplenishmentMethod` |  | object |  |  |  |  |
| `supplyReplenishmentMethod.id` | Internal identifier | string |  |  |  | `TIME_PHASED`, `MPS`, `REORDER_POINT`, `MRP` |
| `supplyReplenishmentMethod.refName` | Reference Name | string |  |  |  |  |
| `supplyTimeFence` | Planning Time Fence | integer | int64 |  |  |  |
| `supplyType` |  | object |  |  |  |  |
| `supplyType.id` | Internal identifier | string |  |  |  | `TRANSFER`, `PURCHASE` |
| `supplyType.refName` | Reference Name | string |  |  |  |  |
| `taxSchedule` |  | taxSchedule |  |  | [`taxSchedule`](taxSchedule.md#taxschedule) |  |
| `totalValue` | Total Value | number | double |  |  |  |
| `trackLandedCost` | Track Landed Cost | boolean |  |  |  |  |
| `tracksaasmetrics` | SaaS Metric Tracking | boolean |  |  |  |  |
| `tracksaasmetricsenddate` | SaaS Metric End Date | string | date |  |  |  |
| `tracksaasmetricsstartdate` | SaaS Metric Start Date | string | date |  |  |  |
| `transferPrice` | Transfer Price | number | double |  |  |  |
| `transferPriceUnits` | Transfer Price Units | string |  |  |  |  |
| `translations` |  | serializedInventoryItem-translationsCollection |  |  | [`serializedInventoryItem-translationsCollection`](#serializedinventoryitem-translationscollection) |  |
| `unitsForPickDecomposition` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `unitsType` |  | unitsType |  |  | [`unitsType`](unitsType.md#unitstype) |  |
| `upcCode` | UPC Code | string |  |  |  |  |
| `updateExistingTranAccounts` | Update Existing Transactions' Accounts | boolean |  |  |  |  |
| `upperWarningLimit` | Upper Warning Limit % (+) | number | float |  |  |  |
| `urlComponent` | URL Component | string |  |  |  |  |
| `useBins` | Use Bins | boolean |  |  |  |  |
| `useMarginalRates` | Use Marginal Rates | boolean |  |  |  |  |
| `vendReturnVarianceAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `vendor` |  | vendor |  |  | [`vendor`](vendor.md#vendor) |  |
| `vendorName` | Vendor Name/Code | string |  |  |  |  |
| `weight` | Item Weight | number | float |  |  |  |
| `weightUnit` |  | object |  |  |  |  |
| `weightUnit.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `weightUnit.refName` | Reference Name | string |  |  |  |  |
| `weightUnits` | Weight Units | string |  |  |  |  |
| `yahooProductFeed` | Yahoo Shopping Product Feed | boolean |  |  |  |  |

## serializedInventoryItem-accountingBookDetailCollection

Browser definition `serializedInventoryItem-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedInventoryItem-accountingBookDetailElement[] |  |  | [`serializedInventoryItem-accountingBookDetailElement`](#serializedinventoryitem-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedInventoryItem-accountingBookDetailElement

Browser definition `serializedInventoryItem-accountingBookDetailElement`.

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

## serializedInventoryItem-binNumberCollection

Browser definition `serializedInventoryItem-binNumberCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedInventoryItem-binNumberElement[] |  |  | [`serializedInventoryItem-binNumberElement`](#serializedinventoryitem-binnumberelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedInventoryItem-binNumberElement

Browser definition `serializedInventoryItem-binNumberElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `binNumber` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `locationActive` | Location Active | string |  |  |  |  |
| `locationName` | Location | string |  |  |  |  |
| `onHand` | On Hand | number | float |  |  |  |
| `onHandAvail` | Available | number | float |  |  |  |
| `preferredBin` | Preferred | boolean |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## serializedInventoryItem-consignedlocationsCollection

Browser definition `serializedInventoryItem-consignedlocationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedInventoryItem-consignedlocationsElement[] |  |  | [`serializedInventoryItem-consignedlocationsElement`](#serializedinventoryitem-consignedlocationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedInventoryItem-consignedlocationsElement

Browser definition `serializedInventoryItem-consignedlocationsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `combinedAverageCost` | Average Cost (All Inventory) | number | double |  |  |  |
| `combinedOnHandCount` | Quantity On Hand (All Inventory) | number | float |  |  |  |
| `combinedOnHandCountBase` | Quantity On Hand (All Inventory Base Unit) | number | float |  |  |  |
| `combinedOnHandValue` | Value (All Inventory) | number | double |  |  |  |
| `consignedAverageCost` | Average Cost (Consigned) | number | double |  |  |  |
| `consignedOnHandCount` | Quantity On Hand (Consigned) | number | float |  |  |  |
| `consignedOnHandCountBase` | Quantity On Hand (Consigned Base Unit) | number | float |  |  |  |
| `consignedOnHandValue` | Value (Consigned) | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `refName` | Reference Name | string |  |  |  |  |

## serializedInventoryItem-correlatedItemsCollection

Browser definition `serializedInventoryItem-correlatedItemsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedInventoryItem-correlatedItemsElement[] |  |  | [`serializedInventoryItem-correlatedItemsElement`](#serializedinventoryitem-correlateditemselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedInventoryItem-correlatedItemsElement

Browser definition `serializedInventoryItem-correlatedItemsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `correlationFld` | Correlation % | number | double |  |  |  |
| `countFld` | Count | integer | int64 |  |  |  |
| `itemNKeyFld` | Item | string |  |  |  |  |
| `liftFld` | Lift % | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `purchaseRateFld` | Overall Purchase Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## serializedInventoryItem-hierarchyVersionsCollection

Browser definition `serializedInventoryItem-hierarchyVersionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedInventoryItem-hierarchyVersionsElement[] |  |  | [`serializedInventoryItem-hierarchyVersionsElement`](#serializedinventoryitem-hierarchyversionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedInventoryItem-hierarchyVersionsElement

Browser definition `serializedInventoryItem-hierarchyVersionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `endDate` | Hierarchy Version End Date | string | date |  |  |  |
| `hierarchyNode` |  | merchandiseHierarchyNode |  |  | [`merchandiseHierarchyNode`](merchandiseHierarchyNode.md#merchandisehierarchynode) |  |
| `hierarchyVersion` |  | merchandiseHierarchyVersion |  |  | [`merchandiseHierarchyVersion`](merchandiseHierarchyVersion.md#merchandisehierarchyversion) |  |
| `isIncluded` | Included In Version | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `startDate` | Hierarchy Version Start Date | string | date |  |  |  |

## serializedInventoryItem-itemVendor-itemVendorPrice

Browser definition `serializedInventoryItem-itemVendor-itemVendorPrice`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `externalId` | External ID | string |  |  |  |  |
| `itemvendorpricelines` |  | serializedInventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection |  |  | [`serializedInventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](#serializedinventoryitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## serializedInventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection

Browser definition `serializedInventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedInventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement[] |  |  | [`serializedInventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](#serializedinventoryitem-itemvendor-itemvendorprice-itemvendorpricelineselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedInventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement

Browser definition `serializedInventoryItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `vendorCost` | Vendor Cost | number | double |  |  |  |
| `vendorcurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `vendorprice` | Purchase Price | number | double |  |  |  |

## serializedInventoryItem-itemVendorCollection

Browser definition `serializedInventoryItem-itemVendorCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedInventoryItem-itemVendorElement[] |  |  | [`serializedInventoryItem-itemVendorElement`](#serializedinventoryitem-itemvendorelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedInventoryItem-itemVendorElement

Browser definition `serializedInventoryItem-itemVendorElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `itemVendorPrice` |  | serializedInventoryItem-itemVendor-itemVendorPrice |  |  | [`serializedInventoryItem-itemVendor-itemVendorPrice`](#serializedinventoryitem-itemvendor-itemvendorprice) |  |
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

## serializedInventoryItem-locationsCollection

Browser definition `serializedInventoryItem-locationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedInventoryItem-locationsElement[] |  |  | [`serializedInventoryItem-locationsElement`](#serializedinventoryitem-locationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedInventoryItem-locationsElement

Browser definition `serializedInventoryItem-locationsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `advanceWarningThreshold` | Firm/Release Advance Warning Threshold | integer | int64 |  |  |  |
| `atpLeadTime` | ATP Lead Time | integer | int64 |  |  |  |
| `averageCostMli` | Average Cost | number | double |  |  |  |
| `backwardConsumptionDays` | Backward Consumption Days | integer | int64 |  |  |  |
| `cost` | Default Cost | number | double |  |  |  |
| `costAccountingStatus` | Cost Accounting Status | string |  |  |  |  |
| `costingLotSize` | Costing Lot Size | number | float |  |  |  |
| `currentStandardCost` | Current Standard Cost | number | double |  |  |  |
| `currentStandardCostEffectiveDate` | Current Standard Cost Effective Date | string | date |  |  |  |
| `defaultReturnCost` | Default Return Cost | number | double |  |  |  |
| `demandSource` |  | object |  |  |  |  |
| `demandSource.id` | Internal identifier | string |  |  |  | `FORECASTANDORDERS`, `EXISTINGORDERSANDDEPENDENTDEMAND`, `FORECASTCONSUMPTION`, `ITEMDEMANDPLAN` |
| `demandSource.refName` | Reference Name | string |  |  |  |  |
| `demandTimeFence` | Demand Time Fence | integer | int64 |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `fixedLotMultiple` | Fixed Lot Multiple | number | float |  |  |  |
| `fixedLotSize` | Fixed Lot Size | number | float |  |  |  |
| `forwardConsumptionDays` | Forward Consumption Days | integer | int64 |  |  |  |
| `inventoryCostTemplate` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `invtClassification` |  | object |  |  |  |  |
| `invtClassification.id` | Internal identifier | string |  |  |  | `1`, `2`, `3` |
| `invtClassification.refName` | Reference Name | string |  |  |  |  |
| `invtCountInterval` | Count Interval | integer | int64 |  |  |  |
| `lastInvtCountDate` | Last Count Date | string | date |  |  |  |
| `lastPurchasePriceMli` | Last Purchase Price | number | double |  |  |  |
| `lateDemandThreshold` | High Impact Late Demand Threshold | number | float |  |  |  |
| `latePeriodDays` | Late Period Days | integer | int64 |  |  |  |
| `leadTime` | Purchase Lead Time | integer | int64 |  |  |  |
| `leadTimeOffset` | Lead Time Offset | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `locationAllowStorePickup` | Allow Store Pickup | boolean |  |  |  |  |
| `locationCostingGroup` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `locationId` | Location | integer | int64 |  |  |  |
| `locationStorePickupBufferStock` | Store Pickup Buffer Stock | number | float |  |  |  |
| `location_display` | Location | string |  |  |  |  |
| `locationqtyavailforstorepickup` | Quantity Available for Store Pickup | number | float |  |  |  |
| `minimumOrderQuantity` | Minimum Order Quantity | number | float |  |  |  |
| `minimumRescheduleDays` | Minimum Reschedule Days | integer | int64 |  |  |  |
| `nextInvtCountDate` | Next Count Date | string | date |  |  |  |
| `onHandValueMli` | Value | number | double |  |  |  |
| `pastDueForecastDays` | Past Due Forecast Days | integer | int64 |  |  |  |
| `periodicLotSizeDays` | Periods of Supply Increment | integer | int64 |  |  |  |
| `periodicLotSizeType` |  | object |  |  |  |  |
| `periodicLotSizeType.id` | Internal identifier | string |  |  |  | `INTERVAL`, `WEEKLY`, `MONTHLY` |
| `periodicLotSizeType.refName` | Reference Name | string |  |  |  |  |
| `poReceiptCost` | PO Receipt Cost | number | double |  |  |  |
| `preferredStockLevel` | Preferred Stock Level | number | float |  |  |  |
| `qtyInTransitExternal` | Quantity In Transit (External) | number | float |  |  |  |
| `quantityAvailable` | Quantity Available | number | float |  |  |  |
| `quantityAvailableBase` | Quantity Available (Base Unit) | number | float |  |  |  |
| `quantityBackOrdered` | Quantity Back Ordered | number | float |  |  |  |
| `quantityCommitted` | Quantity Committed | number | float |  |  |  |
| `quantityInTransit` | Quantity In Transit | number | float |  |  |  |
| `quantityOnHand` | Quantity On Hand | number | float |  |  |  |
| `quantityOnHandBase` | Quantity On Hand (Base Unit) | number | float |  |  |  |
| `quantityOnOrder` | Quantity On Order | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reorderPoint` | Reorder Point | number | float |  |  |  |
| `rescheduleHorizon` | Reschedule Horizon | integer | int64 |  |  |  |
| `rescheduleInDays` | Reschedule In Days | integer | int64 |  |  |  |
| `rescheduleOutDays` | Reschedule Out Days | integer | int64 |  |  |  |
| `safetyStockLevel` | Safety Stock Level | number | float |  |  |  |
| `savedReorderPoint` | Reorder Point | number | float |  |  |  |
| `serialNumbers` | Serial Numbers | string |  |  |  |  |
| `supplyLotSizingMethod` |  | object |  |  |  |  |
| `supplyLotSizingMethod.id` | Internal identifier | string |  |  |  | `FIXED_LOT_SIZE`, `LOT_FOR_LOT`, `FIXED_LOT_MULTIPLE`, `PERIODIC_LOT_SIZE` |
| `supplyLotSizingMethod.refName` | Reference Name | string |  |  |  |  |
| `supplyTimeFence` | Planning Time Fence | integer | int64 |  |  |  |
| `supplyType` |  | object |  |  |  |  |
| `supplyType.id` | Internal identifier | string |  |  |  | `TRANSFER`, `PURCHASE` |
| `supplyType.refName` | Reference Name | string |  |  |  |  |

## serializedInventoryItem-numbersCollection

Browser definition `serializedInventoryItem-numbersCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedInventoryItem-numbersElement[] |  |  | [`serializedInventoryItem-numbersElement`](#serializedinventoryitem-numberselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedInventoryItem-numbersElement

Browser definition `serializedInventoryItem-numbersElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `inventoryNumber` |  | inventoryNumber |  |  | [`inventoryNumber`](inventoryNumber.md#inventorynumber) |  |
| `inventoryNumberId` | Internal ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `quantityOnHand` | On Hand | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `serialNumber` | Serial/Lot Number | string |  |  |  |  |

## serializedInventoryItem-presentationItemCollection

Browser definition `serializedInventoryItem-presentationItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedInventoryItem-presentationItemElement[] |  |  | [`serializedInventoryItem-presentationItemElement`](#serializedinventoryitem-presentationitemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedInventoryItem-presentationItemElement

Browser definition `serializedInventoryItem-presentationItemElement`.

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

## serializedInventoryItem-price

Browser definition `serializedInventoryItem-price`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedInventoryItem-priceElement[] |  |  | [`serializedInventoryItem-priceElement`](#serializedinventoryitem-priceelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedInventoryItem-priceElement

Browser definition `serializedInventoryItem-priceElement`.

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

## serializedInventoryItem-siteCategoryCollection

Browser definition `serializedInventoryItem-siteCategoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedInventoryItem-siteCategoryElement[] |  |  | [`serializedInventoryItem-siteCategoryElement`](#serializedinventoryitem-sitecategoryelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedInventoryItem-siteCategoryElement

Browser definition `serializedInventoryItem-siteCategoryElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `category` |  | siteCategory |  |  | [`siteCategory`](siteCategory.md#sitecategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `webSite` |  | webSite |  |  | [`webSite`](webSite.md#website) |  |

## serializedInventoryItem-translationsCollection

Browser definition `serializedInventoryItem-translationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedInventoryItem-translationsElement[] |  |  | [`serializedInventoryItem-translationsElement`](#serializedinventoryitem-translationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedInventoryItem-translationsElement

Browser definition `serializedInventoryItem-translationsElement`.

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

## serializedInventoryItemCollection

Browser definition `serializedInventoryItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | serializedInventoryItem[] |  |  | [`serializedInventoryItem`](#serializedinventoryitem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedInventoryItemSelectOptions

Browser definition `serializedInventoryItemSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `VSOEDeferral` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `VSOEPermitDiscount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `VSOESopGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `alternateDemandSourceItem` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `amortizationTemplate` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `assetAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `atpMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `baseUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billExchRateVarianceAcct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billPriceVarianceAcct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billQtyVarianceAcct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `billingSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `cogsAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `consignmentassetaccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `consignmentexpenseaccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `consumptionUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `costCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `costingMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `countryOfManufacture` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createExpensePlansOn` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createRevenuePlansOn` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `custReturnVarianceAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultAllocationStrategy` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultItemShipMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deferralAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deferredRevenueAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `demandSource` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `distributionCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `distributionNetwork` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `dropShipExpenseAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `expenseAmortizationRule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `fraudRisk` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `gainLossAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `hazmatPackingGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `incomeAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `insertItemAttribute` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `interCoDefRevAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `intercoCogsAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `intercoIncomeAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `invtClassification` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `issueProduct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemCarrier` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemOptions` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemProcessFamily` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemProcessGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemRevenueCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemShipMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `itemType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `matrixType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `outOfStockBehavior` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `overallQuantityPricingType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `periodicLotSizeType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `planningItemCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `preferenceCriterion` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `preferredLocation` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `pricingGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `purchasePriceVarianceAcct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `purchaseTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `purchaseUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `quantityPricingSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revRecForecastRule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revRecSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revReclassFxAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revenueAllocationGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `revenueRecognitionRule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `rotationType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `saleUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `salesTaxCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `scheduleBCode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `secondaryBaseUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `secondaryConsumptionUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `secondaryPurchaseUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `secondarySaleUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `secondaryStockUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `secondaryUnitsType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipPackage` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `siteMapPriority` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `softDescriptor` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `stockUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `storeDisplayImage` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `storeDisplayThumbnail` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `storeItemTemplate` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `supplyLotSizingMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `supplyReplenishmentMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `supplyType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxSchedule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `unitsForPickDecomposition` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `unitsType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `vendReturnVarianceAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `vendor` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `weightUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

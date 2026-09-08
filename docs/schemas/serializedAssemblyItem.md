# Schemas: serializedAssemblyItem

Property tables for definitions owned by `serializedAssemblyItem`.

Record page: [serializedAssemblyItem](../records/serializedAssemblyItem.md).

## Index

- [serializedAssemblyItem](#serializedassemblyitem) — 332 properties
- [serializedAssemblyItem-accountingBookDetailCollection](#serializedassemblyitem-accountingbookdetailcollection) — 6 properties
- [serializedAssemblyItem-accountingBookDetailElement](#serializedassemblyitem-accountingbookdetailelement) — 11 properties
- [serializedAssemblyItem-billOfMaterialsCollection](#serializedassemblyitem-billofmaterialscollection) — 6 properties
- [serializedAssemblyItem-billOfMaterialsElement](#serializedassemblyitem-billofmaterialselement) — 10 properties
- [serializedAssemblyItem-binNumberCollection](#serializedassemblyitem-binnumbercollection) — 6 properties
- [serializedAssemblyItem-binNumberElement](#serializedassemblyitem-binnumberelement) — 9 properties
- [serializedAssemblyItem-consignedlocationsCollection](#serializedassemblyitem-consignedlocationscollection) — 6 properties
- [serializedAssemblyItem-consignedlocationsElement](#serializedassemblyitem-consignedlocationselement) — 11 properties
- [serializedAssemblyItem-correlatedItemsCollection](#serializedassemblyitem-correlateditemscollection) — 6 properties
- [serializedAssemblyItem-correlatedItemsElement](#serializedassemblyitem-correlateditemselement) — 7 properties
- [serializedAssemblyItem-hierarchyVersionsCollection](#serializedassemblyitem-hierarchyversionscollection) — 6 properties
- [serializedAssemblyItem-hierarchyVersionsElement](#serializedassemblyitem-hierarchyversionselement) — 7 properties
- [serializedAssemblyItem-itemVendor-itemVendorPrice](#serializedassemblyitem-itemvendor-itemvendorprice) — 4 properties
- [serializedAssemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection](#serializedassemblyitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) — 6 properties
- [serializedAssemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement](#serializedassemblyitem-itemvendor-itemvendorprice-itemvendorpricelineselement) — 6 properties
- [serializedAssemblyItem-itemVendorCollection](#serializedassemblyitem-itemvendorcollection) — 6 properties
- [serializedAssemblyItem-itemVendorElement](#serializedassemblyitem-itemvendorelement) — 13 properties
- [serializedAssemblyItem-locationsCollection](#serializedassemblyitem-locationscollection) — 6 properties
- [serializedAssemblyItem-locationsElement](#serializedassemblyitem-locationselement) — 77 properties
- [serializedAssemblyItem-memberCollection](#serializedassemblyitem-membercollection) — 6 properties
- [serializedAssemblyItem-memberElement](#serializedassemblyitem-memberelement) — 20 properties
- [serializedAssemblyItem-numbersCollection](#serializedassemblyitem-numberscollection) — 6 properties
- [serializedAssemblyItem-numbersElement](#serializedassemblyitem-numberselement) — 7 properties
- [serializedAssemblyItem-presentationItemCollection](#serializedassemblyitem-presentationitemcollection) — 6 properties
- [serializedAssemblyItem-presentationItemElement](#serializedassemblyitem-presentationitemelement) — 11 properties
- [serializedAssemblyItem-price](#serializedassemblyitem-price) — 6 properties
- [serializedAssemblyItem-priceElement](#serializedassemblyitem-priceelement) — 10 properties
- [serializedAssemblyItem-siteCategoryCollection](#serializedassemblyitem-sitecategorycollection) — 6 properties
- [serializedAssemblyItem-siteCategoryElement](#serializedassemblyitem-sitecategoryelement) — 4 properties
- [serializedAssemblyItem-translationsCollection](#serializedassemblyitem-translationscollection) — 6 properties
- [serializedAssemblyItem-translationsElement](#serializedassemblyitem-translationselement) — 16 properties
- [serializedAssemblyItemCollection](#serializedassemblyitemcollection) — 6 properties
- [serializedAssemblyItemSelectOptions](#serializedassemblyitemselectoptions) — 97 properties

## serializedAssemblyItem

Browser definition `serializedAssemblyItem`.

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
| `accountingBookDetail` |  | serializedAssemblyItem-accountingBookDetailCollection |  |  | [`serializedAssemblyItem-accountingBookDetailCollection`](#serializedassemblyitem-accountingbookdetailcollection) |  |
| `allowconsignment` | Allow Vendor Consignment | boolean |  |  |  |  |
| `alternateDemandSourceItem` |  | serializedAssemblyItem |  |  | [`serializedAssemblyItem`](#serializedassemblyitem) |  |
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
| `autoProductionLeadTime` | Auto Calculate Production Lead Time | boolean |  |  |  |  |
| `autoReorderPoint` | Auto-Calculate Reorder Point | boolean |  |  |  |  |
| `availableToPartners` | Available to Adv. Partners | boolean |  |  |  |  |
| `averageCost` | Average Cost | number | double |  |  |  |
| `backwardConsumptionDays` | Backward Consumption Days | integer | int64 |  |  |  |
| `baseUnit` | Primary Base Unit | string |  |  |  |  |
| `billExchRateVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `billOfMaterials` |  | serializedAssemblyItem-billOfMaterialsCollection |  |  | [`serializedAssemblyItem-billOfMaterialsCollection`](#serializedassemblyitem-billofmaterialscollection) |  |
| `billPriceVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `billQtyVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `billingSchedule` |  | billingSchedule |  |  | [`billingSchedule`](billingSchedule.md#billingschedule) |  |
| `binNumber` |  | serializedAssemblyItem-binNumberCollection |  |  | [`serializedAssemblyItem-binNumberCollection`](#serializedassemblyitem-binnumbercollection) |  |
| `buildEntireAssembly` | Mark Sub-assemblies Phantom | boolean |  |  |  |  |
| `buildTime` | Work Order Variable Lead Time | number | float |  |  |  |
| `buildTimeLotSize` | Work Order Lead Time Lot Size | number | float |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `cogsAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `consignedlocations` |  | serializedAssemblyItem-consignedlocationsCollection |  |  | [`serializedAssemblyItem-consignedlocationsCollection`](#serializedassemblyitem-consignedlocationscollection) |  |
| `consignmentassetaccount` |  | account |  |  | [`account`](account.md#account) |  |
| `consignmentexpenseaccount` |  | account |  |  | [`account`](account.md#account) |  |
| `consumptionUnit` | Primary Consumption Unit | string |  |  |  |  |
| `contingentRevenueHandling` | Eligible For Contingent Revenue Handling | boolean |  |  |  |  |
| `copyDescription` | Copy from Sales Order | boolean |  |  |  |  |
| `correlatedItems` |  | serializedAssemblyItem-correlatedItemsCollection |  |  | [`serializedAssemblyItem-correlatedItemsCollection`](#serializedassemblyitem-correlateditemscollection) |  |
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
| `defaultAllocationStrategy` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `defaultItemShipMethod` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
| `defaultReturnCost` | Default Return Cost | number | double |  |  |  |
| `defaultReturnCostUnits` |  | string |  |  |  |  |
| `defaultRevision` | Default Revision | string |  |  |  |  |
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
| `effectiveBomControl` |  | object |  |  |  |  |
| `effectiveBomControl.id` | Internal identifier | string |  |  |  | `EFFECTIVE_DATE`, `REVISION_CONTROL` |
| `effectiveBomControl.refName` | Reference Name | string |  |  |  |  |
| `enforceminqtyinternally` | Enforce Minimum Internally | boolean |  |  |  |  |
| `excludeFromSiteMap` | Exclude from Sitemap | boolean |  |  |  |  |
| `expenseAmortizationRule` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `featuredDescription` | Featured Description | string |  |  |  |  |
| `fixedBuildTime` | Work Order Fixed Lead Time | number | float |  |  |  |
| `fixedLotSize` | Fixed Lot Size | number | float |  |  |  |
| `fixedLotSizeUnits` |  | string |  |  |  |  |
| `forwardConsumptionDays` | Forward Consumption Days | integer | int64 |  |  |  |
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
| `hierarchyVersions` |  | serializedAssemblyItem-hierarchyVersionsCollection |  |  | [`serializedAssemblyItem-hierarchyVersionsCollection`](#serializedassemblyitem-hierarchyversionscollection) |  |
| `id` | Internal ID | string |  |  |  |  |
| `includeChildren` | Include Children | boolean |  |  |  |  |
| `incomeAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `insertItemAttribute` |  | object |  |  |  |  |
| `insertItemAttribute.id` | Internal identifier | string |  |  |  | `class`, `department`, `location`, `itemid`, `issueproduct`, `vendorname` |
| `insertItemAttribute.refName` | Reference Name | string |  |  |  |  |
| `intercoCogsAccount` |  | account |  |  | [`account`](account.md#account) |  |
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
| `isPhantom` | Phantom | boolean |  |  |  |  |
| `isSerialItem` | Serialized | boolean |  |  |  |  |
| `isSpecialOrderItem` | Special Order Item | boolean |  |  |  |  |
| `isSpecialWorkOrderItem` | Special Work Order Item | boolean |  |  |  |  |
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
| `itemVendor` |  | serializedAssemblyItem-itemVendorCollection |  |  | [`serializedAssemblyItem-itemVendorCollection`](#serializedassemblyitem-itemvendorcollection) |  |
| `lastInvtCountDate` | Last Count Date | string | date |  |  |  |
| `lastModifiedDate` | Last Modified | string | date-time |  |  |  |
| `lastPurchasePrice` | Last Purchase Price | number | double |  |  |  |
| `leadTime` | Purchase Lead Time | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `locations` |  | serializedAssemblyItem-locationsCollection |  |  | [`serializedAssemblyItem-locationsCollection`](#serializedassemblyitem-locationscollection) |  |
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
| `member` |  | serializedAssemblyItem-memberCollection |  |  | [`serializedAssemblyItem-memberCollection`](#serializedassemblyitem-membercollection) |  |
| `metaTagHtml` | Meta Tag HTML | string |  |  |  |  |
| `minimumquantity` | Minimum Order Qty | integer | int64 |  |  |  |
| `mpn` | Manufacturer Part Number | string |  |  |  |  |
| `multManufactureAddr` | Multiple Manufacturer Addresses | boolean |  |  |  |  |
| `nexTagCategory` | NexTag Category | string |  |  |  |  |
| `nexTagProductFeed` | NexTag Product Feed | boolean |  |  |  |  |
| `nextInvtCountDate` | Next Count Date | string | date |  |  |  |
| `noPriceMessage` | No Price Message | string |  |  |  |  |
| `numbers` |  | serializedAssemblyItem-numbersCollection |  |  | [`serializedAssemblyItem-numbersCollection`](#serializedassemblyitem-numberscollection) |  |
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
| `parent` |  | serializedAssemblyItem |  |  | [`serializedAssemblyItem`](#serializedassemblyitem) |  |
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
| `presentationItem` |  | serializedAssemblyItem-presentationItemCollection |  |  | [`serializedAssemblyItem-presentationItemCollection`](#serializedassemblyitem-presentationitemcollection) |  |
| `price` |  | serializedAssemblyItem-price |  |  | [`serializedAssemblyItem-price`](#serializedassemblyitem-price) |  |
| `pricesIncludeTax` | Prices Include Tax | boolean |  |  |  |  |
| `pricingGroup` |  | pricingGroup |  |  | [`pricingGroup`](pricingGroup.md#pricinggroup) |  |
| `printItems` | Print Items | boolean |  |  |  |  |
| `prodPriceVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `prodQtyVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
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
| `reorderPoint` | Build Point | number | float |  |  |  |
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
| `salesTaxCode` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `savedReorderPoint` | Build Point | number | float |  |  |  |
| `scheduleBCode` |  | object |  |  |  |  |
| `scheduleBCode.id` | Internal identifier | string |  |  |  | `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `10`, `32`, `11`, `33`, `12`, `13`, `14`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21` |
| `scheduleBCode.refName` | Reference Name | string |  |  |  |  |
| `scheduleBNumber` | Schedule B Number | string |  |  |  |  |
| `scheduleBQuantity` | Schedule B Quantity | number | float |  |  |  |
| `scrapAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `searchKeywords` | Search Keywords | string |  |  |  |  |
| `seasonalDemand` | Seasonal Demand | boolean |  |  |  |  |
| `serialNumbers` | Serial Numbers | string |  |  |  |  |
| `shipIndividually` | Ships Individually | boolean |  |  |  |  |
| `shipPackage` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `shippingCost` | Shipping Cost | number | double |  |  |  |
| `shoppingDotComCategory` | Shopping.com Category | string |  |  |  |  |
| `shoppingProductFeed` | Shopping Product Feed | boolean |  |  |  |  |
| `shopzillaCategoryId` | Shopzilla Category ID | integer | int64 |  |  |  |
| `shopzillaProductFeed` | Shopzilla Product Feed | boolean |  |  |  |  |
| `showDefaultDonationAmount` | Show Default Amount | boolean |  |  |  |  |
| `siteCategory` |  | serializedAssemblyItem-siteCategoryCollection |  |  | [`serializedAssemblyItem-siteCategoryCollection`](#serializedassemblyitem-sitecategorycollection) |  |
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
| `transferPrice` | Transfer Price | number | double |  |  |  |
| `transferPriceUnits` | Transfer Price Units | string |  |  |  |  |
| `translations` |  | serializedAssemblyItem-translationsCollection |  |  | [`serializedAssemblyItem-translationsCollection`](#serializedassemblyitem-translationscollection) |  |
| `unbuildVarianceAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `unitsForPickDecomposition` |  | nsResourceCollection |  |  | [`nsResourceCollection`](ns.md#nsresourcecollection) |  |
| `unitsType` |  | unitsType |  |  | [`unitsType`](unitsType.md#unitstype) |  |
| `upcCode` | UPC Code | string |  |  |  |  |
| `updateExistingTranAccounts` | Update Existing Transactions' Accounts | boolean |  |  |  |  |
| `urlComponent` | URL Component | string |  |  |  |  |
| `useBins` | Use Bins | boolean |  |  |  |  |
| `useComponentYield` | Use Component Yield | boolean |  |  |  |  |
| `useMarginalRates` | Use Marginal Rates | boolean |  |  |  |  |
| `vendReturnVarianceAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `vendor` |  | vendor |  |  | [`vendor`](vendor.md#vendor) |  |
| `vendorName` | Vendor Name/Code | string |  |  |  |  |
| `weight` | Item Weight | number | float |  |  |  |
| `weightUnit` |  | object |  |  |  |  |
| `weightUnit.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `weightUnit.refName` | Reference Name | string |  |  |  |  |
| `weightUnits` | Weight Units | string |  |  |  |  |
| `wipAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `wipVarianceAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `yahooProductFeed` | Yahoo Shopping Product Feed | boolean |  |  |  |  |

## serializedAssemblyItem-accountingBookDetailCollection

Browser definition `serializedAssemblyItem-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-accountingBookDetailElement[] |  |  | [`serializedAssemblyItem-accountingBookDetailElement`](#serializedassemblyitem-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-accountingBookDetailElement

Browser definition `serializedAssemblyItem-accountingBookDetailElement`.

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

## serializedAssemblyItem-billOfMaterialsCollection

Browser definition `serializedAssemblyItem-billOfMaterialsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-billOfMaterialsElement[] |  |  | [`serializedAssemblyItem-billOfMaterialsElement`](#serializedassemblyitem-billofmaterialselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-billOfMaterialsElement

Browser definition `serializedAssemblyItem-billOfMaterialsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `billOfMaterials` |  | bom |  |  | [`bom`](bom.md#bom) |  |
| `currentRevision` |  | bomRevision |  |  | [`bomRevision`](bomRevision.md#bomrevision) |  |
| `defaultForLocation` |  | locationCollection |  |  | [`locationCollection`](location.md#locationcollection) |  |
| `effectiveEndDate` | Effective End Date | string | date |  |  |  |
| `effectiveStartDate` | Effective Start Date | string | date |  |  |  |
| `inactive` | Inactive | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `masterDefault` | Master Default | boolean |  |  |  |  |
| `memo` | Memo | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## serializedAssemblyItem-binNumberCollection

Browser definition `serializedAssemblyItem-binNumberCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-binNumberElement[] |  |  | [`serializedAssemblyItem-binNumberElement`](#serializedassemblyitem-binnumberelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-binNumberElement

Browser definition `serializedAssemblyItem-binNumberElement`.

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

## serializedAssemblyItem-consignedlocationsCollection

Browser definition `serializedAssemblyItem-consignedlocationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-consignedlocationsElement[] |  |  | [`serializedAssemblyItem-consignedlocationsElement`](#serializedassemblyitem-consignedlocationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-consignedlocationsElement

Browser definition `serializedAssemblyItem-consignedlocationsElement`.

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

## serializedAssemblyItem-correlatedItemsCollection

Browser definition `serializedAssemblyItem-correlatedItemsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-correlatedItemsElement[] |  |  | [`serializedAssemblyItem-correlatedItemsElement`](#serializedassemblyitem-correlateditemselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-correlatedItemsElement

Browser definition `serializedAssemblyItem-correlatedItemsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `correlationFld` | Correlation % | number | double |  |  |  |
| `countFld` | Count | integer | int64 |  |  |  |
| `itemNKeyFld` | Item | string |  |  |  |  |
| `liftFld` | Lift % | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `purchaseRateFld` | Overall Purchase Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## serializedAssemblyItem-hierarchyVersionsCollection

Browser definition `serializedAssemblyItem-hierarchyVersionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-hierarchyVersionsElement[] |  |  | [`serializedAssemblyItem-hierarchyVersionsElement`](#serializedassemblyitem-hierarchyversionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-hierarchyVersionsElement

Browser definition `serializedAssemblyItem-hierarchyVersionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `endDate` | Hierarchy Version End Date | string | date |  |  |  |
| `hierarchyNode` |  | merchandiseHierarchyNode |  |  | [`merchandiseHierarchyNode`](merchandiseHierarchyNode.md#merchandisehierarchynode) |  |
| `hierarchyVersion` |  | merchandiseHierarchyVersion |  |  | [`merchandiseHierarchyVersion`](merchandiseHierarchyVersion.md#merchandisehierarchyversion) |  |
| `isIncluded` | Included In Version | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `startDate` | Hierarchy Version Start Date | string | date |  |  |  |

## serializedAssemblyItem-itemVendor-itemVendorPrice

Browser definition `serializedAssemblyItem-itemVendor-itemVendorPrice`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `externalId` | External ID | string |  |  |  |  |
| `itemvendorpricelines` |  | serializedAssemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection |  |  | [`serializedAssemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`](#serializedassemblyitem-itemvendor-itemvendorprice-itemvendorpricelinescollection) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## serializedAssemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection

Browser definition `serializedAssemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement[] |  |  | [`serializedAssemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`](#serializedassemblyitem-itemvendor-itemvendorprice-itemvendorpricelineselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement

Browser definition `serializedAssemblyItem-itemVendor-itemVendorPrice-itemvendorpricelinesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `vendorCost` | Vendor Cost | number | double |  |  |  |
| `vendorcurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `vendorprice` | Purchase Price | number | double |  |  |  |

## serializedAssemblyItem-itemVendorCollection

Browser definition `serializedAssemblyItem-itemVendorCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-itemVendorElement[] |  |  | [`serializedAssemblyItem-itemVendorElement`](#serializedassemblyitem-itemvendorelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-itemVendorElement

Browser definition `serializedAssemblyItem-itemVendorElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `itemVendorPrice` |  | serializedAssemblyItem-itemVendor-itemVendorPrice |  |  | [`serializedAssemblyItem-itemVendor-itemVendorPrice`](#serializedassemblyitem-itemvendor-itemvendorprice) |  |
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

## serializedAssemblyItem-locationsCollection

Browser definition `serializedAssemblyItem-locationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-locationsElement[] |  |  | [`serializedAssemblyItem-locationsElement`](#serializedassemblyitem-locationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-locationsElement

Browser definition `serializedAssemblyItem-locationsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `advanceWarningThreshold` | Firm/Release Advance Warning Threshold | integer | int64 |  |  |  |
| `atpLeadTime` | ATP Lead Time | integer | int64 |  |  |  |
| `autoProductionLeadTime` | Auto Calculate Production Lead Time | boolean |  |  |  |  |
| `averageCostMli` | Average Cost | number | double |  |  |  |
| `backwardConsumptionDays` | Backward Consumption Days | integer | int64 |  |  |  |
| `buildTime` | Work Order Variable Lead Time | number | float |  |  |  |
| `buildTimeLotSize` | Work Order Lead Time Lot Size | number | float |  |  |  |
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
| `fixedBuildTime` | Work Order Fixed Lead Time | number | float |  |  |  |
| `fixedLotMultiple` | Fixed Lot Multiple | number | float |  |  |  |
| `fixedLotSize` | Fixed Lot Size | number | float |  |  |  |
| `forwardConsumptionDays` | Forward Consumption Days | integer | int64 |  |  |  |
| `inventoryCostTemplate` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `invtClassification` |  | object |  |  |  |  |
| `invtClassification.id` | Internal identifier | string |  |  |  | `1`, `2`, `3` |
| `invtClassification.refName` | Reference Name | string |  |  |  |  |
| `invtCountInterval` | Count Interval | integer | int64 |  |  |  |
| `isWip` | WIP | boolean |  |  |  |  |
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
| `reorderPoint` | Build Point | number | float |  |  |  |
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

## serializedAssemblyItem-memberCollection

Browser definition `serializedAssemblyItem-memberCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-memberElement[] |  |  | [`serializedAssemblyItem-memberElement`](#serializedassemblyitem-memberelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-memberElement

Browser definition `serializedAssemblyItem-memberElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `bomQuantity` | BoM Quantity | string |  |  |  |  |
| `componentYield` | Component Yield | number | double |  |  |  |
| `effectiveDate` | Effective Date | string | date |  |  |  |
| `effectiveRevision` |  | itemRevision |  |  | [`itemRevision`](itemRevision.md#itemrevision) |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemSource` |  | object |  |  |  |  |
| `itemSource.id` | Internal identifier | string |  |  |  | `WORK_ORDER`, `PHANTOM`, `PURCHASE_ORDER`, `STOCK` |
| `itemSource.refName` | Reference Name | string |  |  |  |  |
| `lineNumber` | Line Id | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `memberDescr` | Description | string |  |  |  |  |
| `memberUnit` | Units | string |  |  |  |  |
| `obsoleteDate` | Obsolete Date | string | date |  |  |  |
| `obsoleteRevision` |  | itemRevision |  |  | [`itemRevision`](itemRevision.md#itemrevision) |  |
| `quantity` | Quantity | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `taxCode` | Tax Code | string |  |  |  |  |
| `taxRate` | Tax Rate | number | double |  |  |  |
| `taxSchedule` |  | taxSchedule |  |  | [`taxSchedule`](taxSchedule.md#taxschedule) |  |

## serializedAssemblyItem-numbersCollection

Browser definition `serializedAssemblyItem-numbersCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-numbersElement[] |  |  | [`serializedAssemblyItem-numbersElement`](#serializedassemblyitem-numberselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-numbersElement

Browser definition `serializedAssemblyItem-numbersElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `inventoryNumber` |  | inventoryNumber |  |  | [`inventoryNumber`](inventoryNumber.md#inventorynumber) |  |
| `inventoryNumberId` | Internal ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `quantityOnHand` | On Hand | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `serialNumber` | Serial/Lot Number | string |  |  |  |  |

## serializedAssemblyItem-presentationItemCollection

Browser definition `serializedAssemblyItem-presentationItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-presentationItemElement[] |  |  | [`serializedAssemblyItem-presentationItemElement`](#serializedassemblyitem-presentationitemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-presentationItemElement

Browser definition `serializedAssemblyItem-presentationItemElement`.

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

## serializedAssemblyItem-price

Browser definition `serializedAssemblyItem-price`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-priceElement[] |  |  | [`serializedAssemblyItem-priceElement`](#serializedassemblyitem-priceelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-priceElement

Browser definition `serializedAssemblyItem-priceElement`.

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

## serializedAssemblyItem-siteCategoryCollection

Browser definition `serializedAssemblyItem-siteCategoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-siteCategoryElement[] |  |  | [`serializedAssemblyItem-siteCategoryElement`](#serializedassemblyitem-sitecategoryelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-siteCategoryElement

Browser definition `serializedAssemblyItem-siteCategoryElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `category` |  | siteCategory |  |  | [`siteCategory`](siteCategory.md#sitecategory) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `webSite` |  | webSite |  |  | [`webSite`](webSite.md#website) |  |

## serializedAssemblyItem-translationsCollection

Browser definition `serializedAssemblyItem-translationsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | serializedAssemblyItem-translationsElement[] |  |  | [`serializedAssemblyItem-translationsElement`](#serializedassemblyitem-translationselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItem-translationsElement

Browser definition `serializedAssemblyItem-translationsElement`.

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

## serializedAssemblyItemCollection

Browser definition `serializedAssemblyItemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | serializedAssemblyItem[] |  |  | [`serializedAssemblyItem`](#serializedassemblyitem) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## serializedAssemblyItemSelectOptions

Browser definition `serializedAssemblyItemSelectOptions`.

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
| `effectiveBomControl` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `expenseAmortizationRule` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `gainLossAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `hazmatPackingGroup` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `incomeAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `insertItemAttribute` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
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
| `prodPriceVarianceAcct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `prodQtyVarianceAcct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
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
| `scrapAcct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
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
| `unbuildVarianceAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `unitsForPickDecomposition` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `unitsType` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `vendReturnVarianceAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `vendor` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `weightUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `wipAcct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `wipVarianceAcct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

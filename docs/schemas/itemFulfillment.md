# Schemas: itemFulfillment

Property tables for definitions owned by `itemFulfillment`.

Record page: [itemFulfillment](../records/itemFulfillment.md).

## Index

- [itemFulfillment](#itemfulfillment) — 178 properties
- [itemFulfillment-accountingBookDetailCollection](#itemfulfillment-accountingbookdetailcollection) — 6 properties
- [itemFulfillment-accountingBookDetailElement](#itemfulfillment-accountingbookdetailelement) — 7 properties
- [itemFulfillment-appliedRulesCollection](#itemfulfillment-appliedrulescollection) — 6 properties
- [itemFulfillment-appliedRulesElement](#itemfulfillment-appliedruleselement) — 9 properties
- [itemFulfillment-item-inventoryDetail](#itemfulfillment-item-inventorydetail) — 11 properties
- [itemFulfillment-item-inventoryDetail-inventoryAssignmentCollection](#itemfulfillment-item-inventorydetail-inventoryassignmentcollection) — 6 properties
- [itemFulfillment-item-inventoryDetail-inventoryAssignmentElement](#itemfulfillment-item-inventorydetail-inventoryassignmentelement) — 17 properties
- [itemFulfillment-itemCollection](#itemfulfillment-itemcollection) — 6 properties
- [itemFulfillment-itemElement](#itemfulfillment-itemelement) — 47 properties
- [itemFulfillment-package-packageDetails](#itemfulfillment-package-packagedetails) — 10 properties
- [itemFulfillment-packageCollection](#itemfulfillment-packagecollection) — 6 properties
- [itemFulfillment-packageElement](#itemfulfillment-packageelement) — 8 properties
- [itemFulfillment-packageFedexCollection](#itemfulfillment-packagefedexcollection) — 6 properties
- [itemFulfillment-packageFedexElement](#itemfulfillment-packagefedexelement) — 44 properties
- [itemFulfillment-packageUpsCollection](#itemfulfillment-packageupscollection) — 6 properties
- [itemFulfillment-packageUpsElement](#itemfulfillment-packageupselement) — 25 properties
- [itemFulfillment-packageUspsCollection](#itemfulfillment-packageuspscollection) — 6 properties
- [itemFulfillment-packageUspsElement](#itemfulfillment-packageuspselement) — 19 properties
- [itemFulfillment-returnShippingAddress](#itemfulfillment-returnshippingaddress) — 18 properties
- [itemFulfillment-shipmentDetails](#itemfulfillment-shipmentdetails) — 6 properties
- [itemFulfillment-shipmentPackageCollection](#itemfulfillment-shipmentpackagecollection) — 6 properties
- [itemFulfillment-shipmentPackageElement](#itemfulfillment-shipmentpackageelement) — 52 properties
- [itemFulfillment-shippingAddress](#itemfulfillment-shippingaddress) — 18 properties
- [itemFulfillmentCollection](#itemfulfillmentcollection) — 6 properties
- [itemFulfillmentSelectOptions](#itemfulfillmentselectoptions) — 36 properties

## itemFulfillment

Browser definition `itemFulfillment`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accessibilityTypeFedex` |  | object |  |  |  |  |
| `accessibilityTypeFedex.id` | Internal identifier | string |  |  |  | `ACCESSIBLE`, `INACCESSIBLE` |
| `accessibilityTypeFedex.refName` | Reference Name | string |  |  |  |  |
| `accountingBookDetail` |  | itemFulfillment-accountingBookDetailCollection |  |  | [`itemFulfillment-accountingBookDetailCollection`](#itemfulfillment-accountingbookdetailcollection) |  |
| `ancillaryEndorsementFedex` |  | object |  |  |  |  |
| `ancillaryEndorsementFedex.id` | Internal identifier | string |  |  |  | `ADDRESS_CORRECTION`, `CARRIER_LEAVE_IF_NO_RESPONSE`, `CHANGE_SERVICE`, `FORWARDING_SERVICE`, `RETURN_SERVICE` |
| `ancillaryEndorsementFedex.refName` | Reference Name | string |  |  |  |  |
| `appliedRules` |  | itemFulfillment-appliedRulesCollection |  |  | [`itemFulfillment-appliedRulesCollection`](#itemfulfillment-appliedrulescollection) |  |
| `b13aFilingOptionFedex` |  | object |  |  |  |  |
| `b13aFilingOptionFedex.id` | Internal identifier | string |  |  |  | `NOT_REQUIRED`, `MANUALLY_ATTACHED`, `FILED_ELECTRONICALLY`, `SUMMARY_REPORTING` |
| `b13aFilingOptionFedex.refName` | Reference Name | string |  |  |  |  |
| `b13aStatementDataFedex` | B13A Statement Data | string |  |  |  |  |
| `backupEmailAddressUps` | Backup Email Address | string |  |  |  |  |
| `blanketEndDateUps` | Blanket Period End Date | string | date |  |  |  |
| `blanketStartDateUps` | Blanket Period Start Date | string | date |  |  |  |
| `bookingConfirmationNumFedex` | Booking Confirmation Number | string |  |  |  |  |
| `carrierIdUps` | Carrier Identification Code | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `createdFrom` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `createdFromShipGroup` | Shipping Group Reference Order Id | integer | int64 |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `eccNumberUps` | ECCN | string |  |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `entryNumberUps` | Entry Number | string |  |  |  |  |
| `exchangeRate` | Exchange Rate | number | float |  |  |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `exportTypeUps` |  | object |  |  |  |  |
| `exportTypeUps.id` | Internal identifier | string |  |  |  | `D`, `F`, `M` |
| `exportTypeUps.refName` | Reference Name | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `generateIntegratedShipperLabel` | Integrated Shipping Label | boolean |  |  |  |  |
| `generateReturnLabel` | Integrated Return Label | boolean |  |  |  |  |
| `halAddr1Fedex` | Hold at Location Address Line 1 | string |  |  |  |  |
| `halAddr2Fedex` | Hold at Location Address Line 2 | string |  |  |  |  |
| `halAddr3Fedex` | Hold at Location Address Line 3 | string |  |  |  |  |
| `halCityFedex` | Hold at Location City | string |  |  |  |  |
| `halCountryFedex` | Hold at Location Country | string |  |  |  |  |
| `halPhoneFedex` | Hold at Location Contact Phone Number | string |  |  |  |  |
| `halStateFedex` | Hold at Location State | string |  |  |  |  |
| `halZipFedex` | Hold at Location Zip Code | string |  |  |  |  |
| `handlingCost` | Handling Cost | number | double |  |  |  |
| `hazmatTypeFedex` |  | object |  |  |  |  |
| `hazmatTypeFedex.id` | Internal identifier | string |  |  |  | `HAZMAT`, `DGOODS` |
| `hazmatTypeFedex.refName` | Reference Name | string |  |  |  |  |
| `holdAtLocationFedex` | Hold at Location | boolean |  |  |  |  |
| `homeDeliveryDateFedex` | Home Delivery Date | string | date |  |  |  |
| `homeDeliveryTypeFedex` |  | object |  |  |  |  |
| `homeDeliveryTypeFedex.id` | Internal identifier | string |  |  |  | `EVENING`, `APPOINTMENT`, `DATECERTAIN` |
| `homeDeliveryTypeFedex.refName` | Reference Name | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inBondCodeUps` | In Bond Code | string |  |  |  |  |
| `insideDeliveryFedex` | Inside Delivery | boolean |  |  |  |  |
| `insidePickupFedex` | Inside Pickup | boolean |  |  |  |  |
| `intlExemptionNumFedex` | AES/FTSR Exemption Number | string |  |  |  |  |
| `isBaseCurrency` | Base Currency | boolean |  |  |  |  |
| `isCargoAircraftOnlyFedex` | Cargo Aircraft Only | boolean |  |  |  |  |
| `isRoutedExportTransactionUps` | Routed Export Transaction | boolean |  |  |  |  |
| `item` |  | itemFulfillment-itemCollection |  |  | [`itemFulfillment-itemCollection`](#itemfulfillment-itemcollection) |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `licenseDateUps` | License Date | string | date |  |  |  |
| `licenseExceptionUps` |  | object |  |  |  |  |
| `licenseExceptionUps.id` | Internal identifier | string |  |  |  | `NLR`, `AGR`, `APR`, `AVS`, `BAG`, `CIV`, `CTP`, `ENC`, `GBS`, `GFT`, `GOV`, `KMI`, `LVS`, `RPL`, `TMP`, `TSPA`, `TSR`, `TSU` |
| `licenseExceptionUps.refName` | Reference Name | string |  |  |  |  |
| `licenseNumberUps` | License Number | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `methodOfTransportUps` |  | object |  |  |  |  |
| `methodOfTransportUps.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `10`, `11`, `12`, `13`, `14`, `15` |
| `methodOfTransportUps.refName` | Reference Name | string |  |  |  |  |
| `optionTypeFedex` |  | object |  |  |  |  |
| `optionTypeFedex.id` | Internal identifier | string |  |  |  | `HAZARDOUS_MATERIALS`, `BATTERY`, `ORM_D`, `REPORTABLE_QUANTITIES`, `SMALL_QUANTITY_EXCEPTION`, `LIMITED_QUANTITIES_COMMODITIES` |
| `optionTypeFedex.refName` | Reference Name | string |  |  |  |  |
| `orderId` | Order Id | integer | int64 |  |  |  |
| `orderType` | Order Type | string |  |  |  |  |
| `package` |  | itemFulfillment-packageCollection |  |  | [`itemFulfillment-packageCollection`](#itemfulfillment-packagecollection) |  |
| `packageFedex` |  | itemFulfillment-packageFedexCollection |  |  | [`itemFulfillment-packageFedexCollection`](#itemfulfillment-packagefedexcollection) |  |
| `packageUps` |  | itemFulfillment-packageUpsCollection |  |  | [`itemFulfillment-packageUpsCollection`](#itemfulfillment-packageupscollection) |  |
| `packageUsps` |  | itemFulfillment-packageUspsCollection |  |  | [`itemFulfillment-packageUspsCollection`](#itemfulfillment-packageuspscollection) |  |
| `packedDate` | Packed Date | string | date |  |  |  |
| `partiesToTransactionUps` | Parties to Transaction | boolean |  |  |  |  |
| `partner` |  | partner |  |  | [`partner`](partner.md#partner) |  |
| `pickedDate` | Picked Date | string | date |  |  |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `recipientTaxIdUps` | Recipient Tax Identification Number | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `regulationFedex` |  | object |  |  |  |  |
| `regulationFedex.id` | Internal identifier | string |  |  |  | `ADR`, `DOT`, `IATA`, `ORMD` |
| `regulationFedex.refName` | Reference Name | string |  |  |  |  |
| `requestedBy` |  | fulfillmentRequest |  |  | [`fulfillmentRequest`](fulfillmentRequest.md#fulfillmentrequest) |  |
| `returnAddress` | Return Shipping Address | string |  |  |  |  |
| `returnAddressList` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `returnShipAddr1` | Address1 | string |  |  |  |  |
| `returnShipAddr2` | Address2 | string |  |  |  |  |
| `returnShipCity` | City | string |  |  |  |  |
| `returnShipCountry` | Country | string |  |  |  |  |
| `returnShipMethod` |  | object |  |  |  |  |
| `returnShipMethod.id` | Internal identifier | string |  |  |  | `44`, `45`, `46`, `47`, `48`, `49`, `50`, `51`, `52`, `53`, `10`, `54`, `11`, `55`, `12`, `56`, `13`, `57`, `14`, `58`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21`, `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `32`, `33`, `34`, `35`, `36`, `37`, `38`, `40`, `41`, `42`, `43` |
| `returnShipMethod.refName` | Reference Name | string |  |  |  |  |
| `returnShipState` | State | string |  |  |  |  |
| `returnShipZipCode` | Zip | string |  |  |  |  |
| `returnShippingAddress` |  | itemFulfillment-returnShippingAddress |  |  | [`itemFulfillment-returnShippingAddress`](#itemfulfillment-returnshippingaddress) |  |
| `returnShippingAddress_text` | Return Address | string |  |  |  |  |
| `salesordchannel` |  | string |  |  |  |  |
| `saturdayDeliveryFedex` | Saturday Delivery | boolean |  |  |  |  |
| `saturdayDeliveryUps` | Saturday Delivery | boolean |  |  |  |  |
| `saturdayPickupFedex` | Saturday Pickup | boolean |  |  |  |  |
| `sendBackupEmailUps` | Send Backup Email | boolean |  |  |  |  |
| `sendShipNotifyEmailFedex` | FedEx ShipAlert® | boolean |  |  |  |  |
| `sendShipNotifyEmailUps` | Ship Notification Email Addresses | boolean |  |  |  |  |
| `sendShipperEmailUps` | Shipper Email Address | boolean |  |  |  |  |
| `shipAddress` | Address | string |  |  |  |  |
| `shipAddressList` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `shipCarrier` |  | object |  |  |  |  |
| `shipCarrier.id` | Internal identifier | string |  |  |  |  |
| `shipCarrier.refName` | Reference Name | string |  |  |  |  |
| `shipCompany` | Shipping Addressee | string |  |  |  |  |
| `shipCountry` |  | object |  |  |  |  |
| `shipCountry.id` | Internal identifier | string |  |  |  | `PR`, `PS`, `PT`, `PW`, `PY`, `QA`, `AB`, `AD`, `AE`, `AF`, `AG`, `AI`, `AL`, `AM`, `AN`, `AO`, `AQ`, `AR`, `AS`, `AT`, `RE`, `AU`, `AW`, `AX`, `AZ`, `RO`, `BA`, `BB`, `RS`, `BD`, `BE`, `RU`, `BF`, `BG`, `RW`, `BH`, `BI`, `BJ`, `BL`, `BM`, `BN`, `BO`, `SA`, `BQ`, `SB`, `BR`, `SC`, `BS`, `SD`, `BT`, `SE`, `BV`, `SG`, `BW`, `SH`, `SI`, `BY`, `SJ`, `BZ`, `SK`, `SL`, `SM`, `SN`, `SO`, `CA`, `SR`, `CC`, `SS`, `CD`, `ST`, `CF`, `SV`, `CG`, `CH`, `SX`, `CI`, `SY`, `SZ`, `CK`, `CL`, `CM`, `CN`, `CO`, `CR`, `TC`, `CS`, `TD`, `CU`, `TF`, `CV`, `TG`, `CW`, `TH`, `CX`, `CY`, `TJ`, `CZ`, `TK`, `TL`, `TM`, `TN`, `TO`, `TR`, `TT`, `DE`, `TV`, `TW`, `DJ`, `TZ`, `DK`, `DM`, `DO`, `UA`, `UG`, `DZ`, `UM`, `EA`, `EC`, `US`, `EE`, `EG`, `EH`, `UY`, `UZ`, `VA`, `ER`, `VC`, `ES`, `ET`, `VE`, `VG`, `VI`, `VN`, `VU`, `FI`, `FJ`, `FK`, `FM`, `FO`, `FR`, `WF`, `GA`, `GB`, `WS`, `GD`, `GE`, `GF`, `GG`, `GH`, `GI`, `GL`, `GM`, `GN`, `GP`, `GQ`, `GR`, `GS`, `GT`, `GU`, `GW`, `GY`, `XK`, `HK`, `HM`, `HN`, `HR`, `HT`, `YE`, `HU`, `IC`, `ID`, `YT`, `IE`, `IL`, `IM`, `IN`, `IO`, `ZA`, `IQ`, `IR`, `IS`, `IT`, `ZM`, `JE`, `ZW`, `JM`, `JO`, `JP`, `KE`, `KG`, `KH`, `KI`, `KM`, `KN`, `KP`, `KR`, `KW`, `KY`, `KZ`, `LA`, `LB`, `LC`, `LI`, `LK`, `LR`, `LS`, `LT`, `LU`, `LV`, `LY`, `MA`, `MC`, `MD`, `ME`, `MF`, `MG`, `MH`, `MK`, `ML`, `MM`, `MN`, `MO`, `MP`, `MQ`, `MR`, `MS`, `MT`, `MU`, `MV`, `MW`, `MX`, `MY`, `MZ`, `NA`, `NC`, `NE`, `NF`, `NG`, `NI`, `NL`, `NO`, `NP`, `NR`, `NU`, `NZ`, `OM`, `PA`, `PE`, `PF`, `PG`, `PH`, `PK`, `PL`, `PM`, `PN` |
| `shipCountry.refName` | Reference Name | string |  |  |  |  |
| `shipDateFedex` | Future Ship Date | string | date |  |  |  |
| `shipIsResidential` | Residential Address | boolean |  |  |  |  |
| `shipMethod` |  | shipItem |  |  | [`shipItem`](shipItem.md#shipitem) |  |
| `shipNotifyEmailAddress2Ups` | Ship Notification Email Address 2 | string |  |  |  |  |
| `shipNotifyEmailAddressFedex` | Ship Notification Email Address | string |  |  |  |  |
| `shipNotifyEmailAddressUps` | Ship Notification Email Address | string |  |  |  |  |
| `shipNotifyEmailMessageUps` | Ship Notification Email Message | string |  |  |  |  |
| `shipOverride` | Override | boolean |  |  |  |  |
| `shipPhone` | Shipping Phone | string |  |  |  |  |
| `shipStatus` |  | object |  |  |  |  |
| `shipStatus.id` | Internal identifier | string |  |  |  | `A`, `B`, `C` |
| `shipStatus.refName` | Reference Name | string |  |  |  |  |
| `shipmentDetails` |  | itemFulfillment-shipmentDetails |  |  | [`itemFulfillment-shipmentDetails`](#itemfulfillment-shipmentdetails) |  |
| `shipmentPackage` |  | itemFulfillment-shipmentPackageCollection |  |  | [`itemFulfillment-shipmentPackageCollection`](#itemfulfillment-shipmentpackagecollection) |  |
| `shipmentWeightFedex` | Total Package Weight | number | float |  |  |  |
| `shipmentWeightUps` | Total Package Weight | number | float |  |  |  |
| `shippedDate` | Shipped Date | string | date |  |  |  |
| `shipperEmailAddressUps` | Shipper Email Address | string |  |  |  |  |
| `shippingAddress` |  | itemFulfillment-shippingAddress |  |  | [`itemFulfillment-shippingAddress`](#itemfulfillment-shippingaddress) |  |
| `shippingAddress_text` | Shipping Address | string |  |  |  |  |
| `shippingCost` | Shipping Cost | number | double |  |  |  |
| `signatureHomeDeliveryFedex` | FedEx Home Delivery® | boolean |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `A`, `B`, `C` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `storeOrder` |  | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `termsFreightChargeFedex` | Terms Freight Charge | number | double |  |  |  |
| `termsInsuranceChargeFedex` | Declared Value | number | double |  |  |  |
| `termsOfSaleFedex` |  | object |  |  |  |  |
| `termsOfSaleFedex.id` | Internal identifier | string |  |  |  | `CFR`, `CIF`, `CIP`, `CPT`, `DAP`, `DAT`, `DDP`, `DDU`, `EXW`, `FCA`, `FOB` |
| `termsOfSaleFedex.refName` | Reference Name | string |  |  |  |  |
| `thirdPartyAcctFedex` | 3rd Party Billing Account Number | string |  |  |  |  |
| `thirdPartyAcctUps` | 3rd Party Billing Account Number | string |  |  |  |  |
| `thirdPartyCountryFedex` |  | object |  |  |  |  |
| `thirdPartyCountryFedex.id` | Internal identifier | string |  |  |  | `PR`, `PS`, `PT`, `PW`, `PY`, `QA`, `AB`, `AD`, `AE`, `AF`, `AG`, `AI`, `AL`, `AM`, `AN`, `AO`, `AQ`, `AR`, `AS`, `AT`, `RE`, `AU`, `AW`, `AX`, `AZ`, `RO`, `BA`, `BB`, `RS`, `BD`, `BE`, `RU`, `BF`, `BG`, `RW`, `BH`, `BI`, `BJ`, `BL`, `BM`, `BN`, `BO`, `SA`, `BQ`, `SB`, `BR`, `SC`, `BS`, `SD`, `BT`, `SE`, `BV`, `SG`, `BW`, `SH`, `SI`, `BY`, `SJ`, `BZ`, `SK`, `SL`, `SM`, `SN`, `SO`, `CA`, `SR`, `CC`, `SS`, `CD`, `ST`, `CF`, `SV`, `CG`, `CH`, `SX`, `CI`, `SY`, `SZ`, `CK`, `CL`, `CM`, `CN`, `CO`, `CR`, `TC`, `CS`, `TD`, `CU`, `TF`, `CV`, `TG`, `CW`, `TH`, `CX`, `CY`, `TJ`, `CZ`, `TK`, `TL`, `TM`, `TN`, `TO`, `TR`, `TT`, `DE`, `TV`, `TW`, `DJ`, `TZ`, `DK`, `DM`, `DO`, `UA`, `UG`, `DZ`, `UM`, `EA`, `EC`, `US`, `EE`, `EG`, `EH`, `UY`, `UZ`, `VA`, `ER`, `VC`, `ES`, `ET`, `VE`, `VG`, `VI`, `VN`, `VU`, `FI`, `FJ`, `FK`, `FM`, `FO`, `FR`, `WF`, `GA`, `GB`, `WS`, `GD`, `GE`, `GF`, `GG`, `GH`, `GI`, `GL`, `GM`, `GN`, `GP`, `GQ`, `GR`, `GS`, `GT`, `GU`, `GW`, `GY`, `XK`, `HK`, `HM`, `HN`, `HR`, `HT`, `YE`, `HU`, `IC`, `ID`, `YT`, `IE`, `IL`, `IM`, `IN`, `IO`, `ZA`, `IQ`, `IR`, `IS`, `IT`, `ZM`, `JE`, `ZW`, `JM`, `JO`, `JP`, `KE`, `KG`, `KH`, `KI`, `KM`, `KN`, `KP`, `KR`, `KW`, `KY`, `KZ`, `LA`, `LB`, `LC`, `LI`, `LK`, `LR`, `LS`, `LT`, `LU`, `LV`, `LY`, `MA`, `MC`, `MD`, `ME`, `MF`, `MG`, `MH`, `MK`, `ML`, `MM`, `MN`, `MO`, `MP`, `MQ`, `MR`, `MS`, `MT`, `MU`, `MV`, `MW`, `MX`, `MY`, `MZ`, `NA`, `NC`, `NE`, `NF`, `NG`, `NI`, `NL`, `NO`, `NP`, `NR`, `NU`, `NZ`, `OM`, `PA`, `PE`, `PF`, `PG`, `PH`, `PK`, `PL`, `PM`, `PN` |
| `thirdPartyCountryFedex.refName` | Reference Name | string |  |  |  |  |
| `thirdPartyCountryUps` |  | object |  |  |  |  |
| `thirdPartyCountryUps.id` | Internal identifier | string |  |  |  | `PR`, `PS`, `PT`, `PW`, `PY`, `QA`, `AB`, `AD`, `AE`, `AF`, `AG`, `AI`, `AL`, `AM`, `AN`, `AO`, `AQ`, `AR`, `AS`, `AT`, `RE`, `AU`, `AW`, `AX`, `AZ`, `RO`, `BA`, `BB`, `RS`, `BD`, `BE`, `RU`, `BF`, `BG`, `RW`, `BH`, `BI`, `BJ`, `BL`, `BM`, `BN`, `BO`, `SA`, `BQ`, `SB`, `BR`, `SC`, `BS`, `SD`, `BT`, `SE`, `BV`, `SG`, `BW`, `SH`, `SI`, `BY`, `SJ`, `BZ`, `SK`, `SL`, `SM`, `SN`, `SO`, `CA`, `SR`, `CC`, `SS`, `CD`, `ST`, `CF`, `SV`, `CG`, `CH`, `SX`, `CI`, `SY`, `SZ`, `CK`, `CL`, `CM`, `CN`, `CO`, `CR`, `TC`, `CS`, `TD`, `CU`, `TF`, `CV`, `TG`, `CW`, `TH`, `CX`, `CY`, `TJ`, `CZ`, `TK`, `TL`, `TM`, `TN`, `TO`, `TR`, `TT`, `DE`, `TV`, `TW`, `DJ`, `TZ`, `DK`, `DM`, `DO`, `UA`, `UG`, `DZ`, `UM`, `EA`, `EC`, `US`, `EE`, `EG`, `EH`, `UY`, `UZ`, `VA`, `ER`, `VC`, `ES`, `ET`, `VE`, `VG`, `VI`, `VN`, `VU`, `FI`, `FJ`, `FK`, `FM`, `FO`, `FR`, `WF`, `GA`, `GB`, `WS`, `GD`, `GE`, `GF`, `GG`, `GH`, `GI`, `GL`, `GM`, `GN`, `GP`, `GQ`, `GR`, `GS`, `GT`, `GU`, `GW`, `GY`, `XK`, `HK`, `HM`, `HN`, `HR`, `HT`, `YE`, `HU`, `IC`, `ID`, `YT`, `IE`, `IL`, `IM`, `IN`, `IO`, `ZA`, `IQ`, `IR`, `IS`, `IT`, `ZM`, `JE`, `ZW`, `JM`, `JO`, `JP`, `KE`, `KG`, `KH`, `KI`, `KM`, `KN`, `KP`, `KR`, `KW`, `KY`, `KZ`, `LA`, `LB`, `LC`, `LI`, `LK`, `LR`, `LS`, `LT`, `LU`, `LV`, `LY`, `MA`, `MC`, `MD`, `ME`, `MF`, `MG`, `MH`, `MK`, `ML`, `MM`, `MN`, `MO`, `MP`, `MQ`, `MR`, `MS`, `MT`, `MU`, `MV`, `MW`, `MX`, `MY`, `MZ`, `NA`, `NC`, `NE`, `NF`, `NG`, `NI`, `NL`, `NO`, `NP`, `NR`, `NU`, `NZ`, `OM`, `PA`, `PE`, `PF`, `PG`, `PH`, `PK`, `PL`, `PM`, `PN` |
| `thirdPartyCountryUps.refName` | Reference Name | string |  |  |  |  |
| `thirdPartyTypeFedex` |  | object |  |  |  |  |
| `thirdPartyTypeFedex.id` | Internal identifier | string |  |  |  | `BILLNONESELECTED`, `BILLTHIRDPARTY`, `BILLRECIPIENT`, `BILLCOLLECT` |
| `thirdPartyTypeFedex.refName` | Reference Name | string |  |  |  |  |
| `thirdPartyTypeUps` |  | object |  |  |  |  |
| `thirdPartyTypeUps.id` | Internal identifier | string |  |  |  | `BILLNONESELECTED`, `BILLTHIRDPARTY`, `BILLRECIPIENT`, `BILLCOLLECT` |
| `thirdPartyTypeUps.refName` | Reference Name | string |  |  |  |  |
| `thirdPartyZipCodeUps` | 3rd Party Billing Zip | string |  |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Ref No. | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `transferLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `webSite` |  | string |  |  |  |  |

## itemFulfillment-accountingBookDetailCollection

Browser definition `itemFulfillment-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemFulfillment-accountingBookDetailElement[] |  |  | [`itemFulfillment-accountingBookDetailElement`](#itemfulfillment-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemFulfillment-accountingBookDetailElement

Browser definition `itemFulfillment-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## itemFulfillment-appliedRulesCollection

Browser definition `itemFulfillment-appliedRulesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemFulfillment-appliedRulesElement[] |  |  | [`itemFulfillment-appliedRulesElement`](#itemfulfillment-appliedruleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemFulfillment-appliedRulesElement

Browser definition `itemFulfillment-appliedRulesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `creationDate` | Date | string | date |  |  |  |
| `details` | Details | string |  |  |  |  |
| `externalLogId` | External ID | integer | int64 |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `ruleType` | Rule Type: | string |  |  |  |  |
| `ruleTypeTranslation` | Rule Type | string |  |  |  |  |
| `transactionVersion` | Version | integer | int64 |  |  |  |

## itemFulfillment-item-inventoryDetail

Browser definition `itemFulfillment-item-inventoryDetail`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `externalId` | External ID | string |  |  |  |  |
| `inventoryAssignment` |  | itemFulfillment-item-inventoryDetail-inventoryAssignmentCollection |  |  | [`itemFulfillment-item-inventoryDetail-inventoryAssignmentCollection`](#itemfulfillment-item-inventorydetail-inventoryassignmentcollection) |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemDescription` | Description | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `quantity` | Quantity | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `toLocation` |  | location |  |  | [`location`](location.md#location) |  |
| `unit` | Units | string |  |  |  |  |

## itemFulfillment-item-inventoryDetail-inventoryAssignmentCollection

Browser definition `itemFulfillment-item-inventoryDetail-inventoryAssignmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemFulfillment-item-inventoryDetail-inventoryAssignmentElement[] |  |  | [`itemFulfillment-item-inventoryDetail-inventoryAssignmentElement`](#itemfulfillment-item-inventorydetail-inventoryassignmentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemFulfillment-item-inventoryDetail-inventoryAssignmentElement

Browser definition `itemFulfillment-item-inventoryDetail-inventoryAssignmentElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `binNumber` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `inventoryDetail` | Inventory Detail | integer | int64 |  |  |  |
| `inventoryStatus` |  | inventoryStatus |  |  | [`inventoryStatus`](inventoryStatus.md#inventorystatus) |  |
| `issueInventoryNumber` |  | inventoryNumber |  |  | [`inventoryNumber`](inventoryNumber.md#inventorynumber) |  |
| `licensePlateNumber` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `packCarton` | Pack Carton | string |  |  |  |  |
| `pickCarton` | Pick Carton | string |  |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityAvailable` | Unpicked Bin Qty | number | float |  |  |  |
| `receiptInventoryNumber` | Serial/Lot Number | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `secondaryQuantity` | Secondary Quantity | number | float |  |  |  |
| `toBinNumber` |  | bin |  |  | [`bin`](bin.md#bin) |  |
| `toInventoryStatus` |  | inventoryStatus |  |  | [`inventoryStatus`](inventoryStatus.md#inventorystatus) |  |

## itemFulfillment-itemCollection

Browser definition `itemFulfillment-itemCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemFulfillment-itemElement[] |  |  | [`itemFulfillment-itemElement`](#itemfulfillment-itemelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemFulfillment-itemElement

Browser definition `itemFulfillment-itemElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Amount | number | double |  |  |  |
| `binNumbers` | Bin Numbers | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `consigned` | Consigned | boolean |  |  |  |  |
| `consignmentConsumed` | Consignment Consumed | string |  |  |  |  |
| `createPo` | Drop Ship PO | string |  |  |  |  |
| `createdPo` |  | purchaseOrder |  |  | [`purchaseOrder`](purchaseOrder.md#purchaseorder) |  |
| `currency` | Currency | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `description` | Description | string |  |  |  |  |
| `displayName` | Display Name | string |  |  |  |  |
| `excludeFromRateRequest` | Exclude Item from Rate Request | boolean |  |  |  |  |
| `expirationDate` | Expiration Date | string | date |  |  |  |
| `inventoryDetail` |  | itemFulfillment-item-inventoryDetail |  |  | [`itemFulfillment-item-inventoryDetail`](#itemfulfillment-item-inventorydetail) |  |
| `isCatchWeightItem` |  | boolean |  |  |  |  |
| `isConsignmentItem` |  | boolean |  |  |  |  |
| `item` |  | kitItem |  |  | [`kitItem`](kitItem.md#kititem) |  |
| `itemFxAmount` | Foreign Amount | number | double |  |  |  |
| `itemName` | Item | string |  |  |  |  |
| `itemReceive` | Fulfill/Receive | boolean |  |  |  |  |
| `itemSubtype` | Subtype | string |  |  |  |  |
| `itemType` | Type | string |  |  |  |  |
| `itemUnitPrice` | Unit Price | number | double |  |  |  |
| `itemUpc` | UPC Code | string |  |  |  |  |
| `jobName` | Job | string |  |  |  |  |
| `kitMemberOf` | Member of Line | integer | int64 |  |  |  |
| `line` | Transaction Line | integer | int64 |  |  |  |
| `lineEntity` | Entity | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `onHand` | On Hand | number | float |  |  |  |
| `options` | Options | string |  |  |  |  |
| `orderDoc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `orderLine` | Order Line | integer | int64 |  |  |  |
| `primaryToSecondaryUnitConversionRate` |  | number | float |  |  |  |
| `quantity` | Quantity | number | float |  |  |  |
| `quantityRemaining` | Quantity Remaining | number | float |  |  |  |
| `quantityRemainingDisplay` | Remaining | number | float |  |  |  |
| `rate` | Rate | number | double |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `secondaryQuantity` | Secondary Quantity | number | float |  |  |  |
| `secondaryUnitConversionRate` |  | number | float |  |  |  |
| `secondaryUnits` | Secondary Units | string |  |  |  |  |
| `secondaryUnitsList` |  | string |  |  |  |  |
| `serialNumbers` | Serial/Lot Numbers | string |  |  |  |  |
| `units` | Units | string |  |  |  |  |
| `unitsDisplay` | Units | string |  |  |  |  |

## itemFulfillment-package-packageDetails

Browser definition `itemFulfillment-package-packageDetails`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `declaredValue` | Declared Value | number | double |  |  |  |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `packageHeight` | Height | number | float |  |  |  |
| `packageLength` | Length | number | float |  |  |  |
| `packageWidth` | Width | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## itemFulfillment-packageCollection

Browser definition `itemFulfillment-packageCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemFulfillment-packageElement[] |  |  | [`itemFulfillment-packageElement`](#itemfulfillment-packageelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemFulfillment-packageElement

Browser definition `itemFulfillment-packageElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `packageCartonNumber` | Carton Number | string |  |  |  |  |
| `packageDescr` | Package Contents Description | string |  |  |  |  |
| `packageDetails` |  | itemFulfillment-package-packageDetails |  |  | [`itemFulfillment-package-packageDetails`](#itemfulfillment-package-packagedetails) |  |
| `packageTrackingNumber` | Package Tracking Number | string |  |  |  |  |
| `packageTrackingNumberReturn` | Return Tracking Number | string |  |  |  |  |
| `packageWeight` | Weight in Pounds | number | float |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## itemFulfillment-packageFedexCollection

Browser definition `itemFulfillment-packageFedexCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemFulfillment-packageFedexElement[] |  |  | [`itemFulfillment-packageFedexElement`](#itemfulfillment-packagefedexelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemFulfillment-packageFedexElement

Browser definition `itemFulfillment-packageFedexElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `admPackageTypeFedEx` |  | object |  |  |  |  |
| `admPackageTypeFedEx.id` | Internal identifier | string |  |  |  | `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `10`, `11`, `12`, `13`, `14`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21` |
| `admPackageTypeFedEx.refName` | Reference Name | string |  |  |  |  |
| `alcoholRecipientTypeFedEx` |  | object |  |  |  |  |
| `alcoholRecipientTypeFedEx.id` | Internal identifier | string |  |  |  | `CONSUMER`, `LICENSEE` |
| `alcoholRecipientTypeFedEx.refName` | Reference Name | string |  |  |  |  |
| `authorizationNumberFedEx` | Authorization Number | string |  |  |  |  |
| `codAmountFedEx` | C.O.D. Amount | number | double |  |  |  |
| `codFreightTypeFedEx` |  | object |  |  |  |  |
| `codFreightTypeFedEx.id` | Internal identifier | string |  |  |  | `NONESELECTED`, `NET_CHARGE`, `COD_SURCHARGE`, `TOTAL_CUSTOMER_CHARGE`, `NET_FREIGHT` |
| `codFreightTypeFedEx.refName` | Reference Name | string |  |  |  |  |
| `codMethodFedEx` |  | object |  |  |  |  |
| `codMethodFedEx.id` | Internal identifier | string |  |  |  | `3`, `4`, `5` |
| `codMethodFedEx.refName` | Reference Name | string |  |  |  |  |
| `deliveryConfFedEx` |  | object |  |  |  |  |
| `deliveryConfFedEx.id` | Internal identifier | string |  |  |  | `1`, `2` |
| `deliveryConfFedEx.refName` | Reference Name | string |  |  |  |  |
| `dryIceWeightFedEx` | Dry Ice Weight | number | float |  |  |  |
| `insuredValueFedEx` | Declared Value | number | double |  |  |  |
| `isAlcoholFedEx` | Alcohol | boolean |  |  |  |  |
| `isNonHazLithiumFedEx` | Non-Hazardous Lithium Batteries | boolean |  |  |  |  |
| `isNonStandardContainerFedEx` | Non Standard Container | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `packageCartonNumberFedEx` | Carton Number | string |  |  |  |  |
| `packageHeightFedEx` | Height | integer | int64 |  |  |  |
| `packageLengthFedEx` | Length | integer | int64 |  |  |  |
| `packageTrackingNumberFedEx` | Package Tracking Number | string |  |  |  |  |
| `packageWeightFedEx` | Weight in Pounds | number | float |  |  |  |
| `packageWidthFedEx` | Width | integer | int64 |  |  |  |
| `packagingFedEx` |  | object |  |  |  |  |
| `packagingFedEx.id` | Internal identifier | string |  |  |  | `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `32`, `10`, `33`, `34`, `35`, `14`, `36`, `37`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21` |
| `packagingFedEx.refName` | Reference Name | string |  |  |  |  |
| `priorityAlertContentFedEx` | Content Description | string |  |  |  |  |
| `priorityAlertTypeFedEx` |  | object |  |  |  |  |
| `priorityAlertTypeFedEx.id` | Internal identifier | string |  |  |  | `NONESELECTED`, `PRIORITY_ALERT`, `PRIORITY_ALERT_PLUS` |
| `priorityAlertTypeFedEx.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reference1FedEx` | Reference Information | string |  |  |  |  |
| `signatureOptionsFedEx` |  | object |  |  |  |  |
| `signatureOptionsFedEx.id` | Internal identifier | string |  |  |  | `NONESELECTED`, `PRIORITY_ALERT`, `PRIORITY_ALERT_PLUS` |
| `signatureOptionsFedEx.refName` | Reference Name | string |  |  |  |  |
| `signatureReleaseFedEx` | Signature Release | string |  |  |  |  |
| `useCodFedEx` | C.O.D. Amount | boolean |  |  |  |  |
| `useInsuredValueFedEx` | Declared Value | boolean |  |  |  |  |

## itemFulfillment-packageUpsCollection

Browser definition `itemFulfillment-packageUpsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemFulfillment-packageUpsElement[] |  |  | [`itemFulfillment-packageUpsElement`](#itemfulfillment-packageupselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemFulfillment-packageUpsElement

Browser definition `itemFulfillment-packageUpsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `additionalHandlingUps` | Additional Handling | boolean |  |  |  |  |
| `codAmountUps` | C.O.D. Amount | number | double |  |  |  |
| `codMethodUps` |  | object |  |  |  |  |
| `codMethodUps.id` | Internal identifier | string |  |  |  | `1`, `2` |
| `codMethodUps.refName` | Reference Name | string |  |  |  |  |
| `deliveryConfUps` |  | object |  |  |  |  |
| `deliveryConfUps.id` | Internal identifier | string |  |  |  | `1`, `2`, `3` |
| `deliveryConfUps.refName` | Reference Name | string |  |  |  |  |
| `insuredValueUps` | Insured Value | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `packageCartonNumberUps` | Carton Number | string |  |  |  |  |
| `packageDescrUps` | Package Contents Description | string |  |  |  |  |
| `packageHeightUps` | Height | integer | int64 |  |  |  |
| `packageLengthUps` | Length | integer | int64 |  |  |  |
| `packageTrackingNumberUps` | Package Tracking Number | string |  |  |  |  |
| `packageWeightUps` | Weight in Pounds | number | float |  |  |  |
| `packageWidthUps` | Width | integer | int64 |  |  |  |
| `packagingUps` |  | object |  |  |  |  |
| `packagingUps.id` | Internal identifier | string |  |  |  | `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `32`, `10`, `33`, `34`, `35`, `14`, `36`, `37`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21` |
| `packagingUps.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reference1Ups` | Reference #1 | string |  |  |  |  |
| `reference2Ups` | Reference #2 | string |  |  |  |  |
| `useCodUps` | C.O.D. Amount | boolean |  |  |  |  |
| `useInsuredValueUps` | Declared Value | boolean |  |  |  |  |

## itemFulfillment-packageUspsCollection

Browser definition `itemFulfillment-packageUspsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemFulfillment-packageUspsElement[] |  |  | [`itemFulfillment-packageUspsElement`](#itemfulfillment-packageuspselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemFulfillment-packageUspsElement

Browser definition `itemFulfillment-packageUspsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `deliveryConfUsps` |  | object |  |  |  |  |
| `deliveryConfUsps.id` | Internal identifier | string |  |  |  | `6`, `7` |
| `deliveryConfUsps.refName` | Reference Name | string |  |  |  |  |
| `insuredValueUsps` | Declared Value | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `packageCartonNumberUsps` | Carton Number | string |  |  |  |  |
| `packageDescrUsps` | Package Contents Description | string |  |  |  |  |
| `packageHeightUsps` | Height | integer | int64 |  |  |  |
| `packageLengthUsps` | Length | integer | int64 |  |  |  |
| `packageTrackingNumberUsps` | Package Tracking Number | string |  |  |  |  |
| `packageWeightUsps` | Weight in Pounds | number | float |  |  |  |
| `packageWidthUsps` | Width | integer | int64 |  |  |  |
| `packagingUsps` |  | object |  |  |  |  |
| `packagingUsps.id` | Internal identifier | string |  |  |  | `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `32`, `10`, `33`, `34`, `35`, `14`, `36`, `37`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21` |
| `packagingUsps.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reference1Usps` | Reference #1 | string |  |  |  |  |
| `reference2Usps` | Reference #2 | string |  |  |  |  |
| `useInsuredValueUsps` | Insured Value | boolean |  |  |  |  |

## itemFulfillment-returnShippingAddress

Browser definition `itemFulfillment-returnShippingAddress`.

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

## itemFulfillment-shipmentDetails

Browser definition `itemFulfillment-shipmentDetails`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `description` | Description | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## itemFulfillment-shipmentPackageCollection

Browser definition `itemFulfillment-shipmentPackageCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | itemFulfillment-shipmentPackageElement[] |  |  | [`itemFulfillment-shipmentPackageElement`](#itemfulfillment-shipmentpackageelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemFulfillment-shipmentPackageElement

Browser definition `itemFulfillment-shipmentPackageElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `admissibilityPackageType` |  | object |  |  |  |  |
| `admissibilityPackageType.id` | Internal identifier | string |  |  |  | `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `10`, `11`, `12`, `13`, `14`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21` |
| `admissibilityPackageType.refName` | Reference Name | string |  |  |  |  |
| `alcoholRecipientType` |  | object |  |  |  |  |
| `alcoholRecipientType.id` | Internal identifier | string |  |  |  | `CONSUMER`, `LICENSEE` |
| `alcoholRecipientType.refName` | Reference Name | string |  |  |  |  |
| `authorizationNumber` | Authorization Number | string |  |  |  |  |
| `carrierPackaging` |  | object |  |  |  |  |
| `carrierPackaging.id` | Internal identifier | string |  |  |  | `22`, `23`, `24`, `25`, `26`, `27`, `28`, `29`, `30`, `31`, `32`, `10`, `33`, `34`, `35`, `14`, `36`, `37`, `15`, `16`, `17`, `18`, `19`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`, `20`, `21` |
| `carrierPackaging.refName` | Reference Name | string |  |  |  |  |
| `cashOnDeliveryAmount` | Cash On Delivery Amount | number | double |  |  |  |
| `cashOnDeliveryMethod` |  | object |  |  |  |  |
| `cashOnDeliveryMethod.id` | Internal identifier | string |  |  |  | `3`, `4`, `5` |
| `cashOnDeliveryMethod.refName` | Reference Name | string |  |  |  |  |
| `codOtherCharge` | C.O.D. Other Charge | number | double |  |  |  |
| `contentsDescription` | Contents Description | string |  |  |  |  |
| `declaredValue` | Declared Value | number | double |  |  |  |
| `deliveryConfirmation` |  | object |  |  |  |  |
| `deliveryConfirmation.id` | Internal identifier | string |  |  |  | `1`, `2` |
| `deliveryConfirmation.refName` | Reference Name | string |  |  |  |  |
| `dimensionUnit` | Dimension Unit | string |  |  |  |  |
| `dryIceWeight` | Dry Ice Weight | number | float |  |  |  |
| `freightChargeAddedToCod` |  | object |  |  |  |  |
| `freightChargeAddedToCod.id` | Internal identifier | string |  |  |  | `NONESELECTED`, `NET_CHARGE`, `COD_SURCHARGE`, `TOTAL_CUSTOMER_CHARGE`, `NET_FREIGHT` |
| `freightChargeAddedToCod.refName` | Reference Name | string |  |  |  |  |
| `hasAdditionalHandling` | Has Additional Handling | boolean |  |  |  |  |
| `hasCashOnDelivery` | Has Cash On Delivery | boolean |  |  |  |  |
| `hasDeclaredValue` | Has Declared Value | boolean |  |  |  |  |
| `hasInsuredValue` | Has Insured Value | boolean |  |  |  |  |
| `height` | Height | integer | int64 |  |  |  |
| `insuredValue` | Insured Value | number | double |  |  |  |
| `isAlcohol` | Is Alcohol | boolean |  |  |  |  |
| `isNonHazardousLiBatteries` | Is Non Hazardous Lithium Batteries | boolean |  |  |  |  |
| `isNonStandardContainer` | Is Non Standard Container | boolean |  |  |  |  |
| `length` | Length | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `priorityAlertContent` | Content Description | string |  |  |  |  |
| `priorityAlertType` |  | object |  |  |  |  |
| `priorityAlertType.id` | Internal identifier | string |  |  |  | `NONESELECTED`, `PRIORITY_ALERT`, `PRIORITY_ALERT_PLUS` |
| `priorityAlertType.refName` | Reference Name | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `reference` | Reference | string |  |  |  |  |
| `reference2` | Reference #2 | string |  |  |  |  |
| `sequenceNumber` | Sequence Number | integer | int64 |  |  |  |
| `signatureOption` |  | object |  |  |  |  |
| `signatureOption.id` | Internal identifier | string |  |  |  | `NONESELECTED`, `PRIORITY_ALERT`, `PRIORITY_ALERT_PLUS` |
| `signatureOption.refName` | Reference Name | string |  |  |  |  |
| `signatureRelease` | Signature Release | string |  |  |  |  |
| `trackingNumber` | TrackingNumber | string |  |  |  |  |
| `weightInLbs` | Weight in Pounds | number | float |  |  |  |
| `width` | Width | integer | int64 |  |  |  |
| `yourPackaging` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## itemFulfillment-shippingAddress

Browser definition `itemFulfillment-shippingAddress`.

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

## itemFulfillmentCollection

Browser definition `itemFulfillmentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | itemFulfillment[] |  |  | [`itemFulfillment`](#itemfulfillment) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## itemFulfillmentSelectOptions

Browser definition `itemFulfillmentSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accessibilityTypeFedex` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `ancillaryEndorsementFedex` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `b13aFilingOptionFedex` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `createdFrom` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `entity` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `exportTypeUps` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `hazmatTypeFedex` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `homeDeliveryTypeFedex` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `licenseExceptionUps` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `methodOfTransportUps` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `optionTypeFedex` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `partner` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `regulationFedex` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `requestedBy` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `returnAddressList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `returnShipMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipAddressList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipCarrier` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipCountry` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipMethod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `shipStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `termsOfSaleFedex` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `thirdPartyCountryFedex` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `thirdPartyCountryUps` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `thirdPartyTypeFedex` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `thirdPartyTypeUps` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transferLocation` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

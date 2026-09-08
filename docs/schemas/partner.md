# Schemas: partner

Property tables for definitions owned by `partner`.

Record page: [partner](../records/partner.md).

## Index

- [partner](#partner) — 72 properties
- [partner-addressBook-addressBookAddress](#partner-addressbook-addressbookaddress) — 18 properties
- [partner-addressBookCollection](#partner-addressbookcollection) — 6 properties
- [partner-addressBookElement](#partner-addressbookelement) — 11 properties
- [partner-campaignsCollection](#partner-campaignscollection) — 6 properties
- [partner-campaignsElement](#partner-campaignselement) — 2 properties
- [partner-contactRolesCollection](#partner-contactrolescollection) — 6 properties
- [partner-contactRolesElement](#partner-contactroleselement) — 9 properties
- [partner-subscriptionMessageHistoryCollection](#partner-subscriptionmessagehistorycollection) — 6 properties
- [partner-subscriptionMessageHistoryElement](#partner-subscriptionmessagehistoryelement) — 2 properties
- [partner-subscriptionsCollection](#partner-subscriptionscollection) — 6 properties
- [partner-subscriptionsElement](#partner-subscriptionselement) — 5 properties
- [partner-taxRegistrationCollection](#partner-taxregistrationcollection) — 6 properties
- [partner-taxRegistrationElement](#partner-taxregistrationelement) — 10 properties
- [partnerCollection](#partnercollection) — 6 properties
- [partnerSelectOptions](#partnerselectoptions) — 17 properties

## partner

Browser definition `partner`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accessRole` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `addressBook` |  | partner-addressBookCollection |  |  | [`partner-addressBookCollection`](#partner-addressbookcollection) |  |
| `altEmail` | Alt. Email | string |  |  |  |  |
| `altName` | Partner | string |  |  |  |  |
| `autoName` | Auto | boolean |  |  |  |  |
| `bcn` | Business Number | string |  |  |  |  |
| `campaigns` |  | partner-campaignsCollection |  |  | [`partner-campaignsCollection`](#partner-campaignscollection) |  |
| `category` |  | partnerCategoryCollection |  |  | [`partnerCategoryCollection`](partnerCategory.md#partnercategorycollection) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `comments` | Comments | string |  |  |  |  |
| `companyName` | Company Name | string |  |  |  |  |
| `contact` |  | contact |  |  | [`contact`](contact.md#contact) |  |
| `contactList` |  | contactCollection |  |  | [`contactCollection`](contact.md#contactcollection) |  |
| `contactRoles` |  | partner-contactRolesCollection |  |  | [`partner-contactRolesCollection`](#partner-contactrolescollection) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `dateCreated` | Date Created | string | date-time |  |  |  |
| `defaultAddress` | Default Address | string |  |  |  |  |
| `defaultShippingAddress` | Default Shipping Address | string |  |  |  |  |
| `defaultTaxReg` | Default Tax Reg. Number | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `eligibleForCommission` | Eligible for Commission | boolean |  |  |  |  |
| `email` | Partner Email | string |  |  |  |  |
| `emailPreference` |  | object |  |  |  |  |
| `emailPreference.id` | Internal identifier | string |  |  |  | `PDF`, `HTML`, `DEFAULT` |
| `emailPreference.refName` | Reference Name | string |  |  |  |  |
| `entityId` | Entity ID | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fax` | Fax | string |  |  |  |  |
| `firstName` | First Name | string |  |  |  |  |
| `giveAccess` | Login Access | boolean |  |  |  |  |
| `globalSubscriptionStatus` |  | object |  |  |  |  |
| `globalSubscriptionStatus.id` | Internal identifier | string |  |  |  | `1`, `2`, `3`, `4` |
| `globalSubscriptionStatus.refName` | Reference Name | string |  |  |  |  |
| `homePhone` | Home Phone | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `image` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `isInactive` | Inactive | boolean |  |  |  |  |
| `isPerson` | Is Individual | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `lastName` | Last Name | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `middleName` | Middle Name | string |  |  |  |  |
| `mobilePhone` | Mobile Phone | string |  |  |  |  |
| `parent` |  | partner |  |  | [`partner`](#partner) |  |
| `partnerCode` | Partner Code | string |  |  |  |  |
| `password` | Password | string |  |  |  |  |
| `password2` | Confirm Password | string |  |  |  |  |
| `phone` | Phone | string |  |  |  |  |
| `phoneticName` | Furigana | string |  |  |  |  |
| `printOnCheckAs` | Print on Check As | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `referringUrl` | Referring URL | string |  |  |  |  |
| `requirePwdChange` | Require Password Change On Next Login | boolean |  |  |  |  |
| `salutation` | Mr./Ms... | string |  |  |  |  |
| `sendEmail` | Send New Access Notification Email | boolean |  |  |  |  |
| `subpartnerLogin` | Can give login access to sub-partners | boolean |  |  |  |  |
| `subscriptionMessageHistory` |  | partner-subscriptionMessageHistoryCollection |  |  | [`partner-subscriptionMessageHistoryCollection`](#partner-subscriptionmessagehistorycollection) |  |
| `subscriptions` |  | partner-subscriptionsCollection |  |  | [`partner-subscriptionsCollection`](#partner-subscriptionscollection) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `taxFractionUnit` |  | object |  |  |  |  |
| `taxFractionUnit.id` | Internal identifier | string |  |  |  | `2`, `1`, `0`, `-1`, `-2` |
| `taxFractionUnit.refName` | Reference Name | string |  |  |  |  |
| `taxIdNum` | Tax ID | string |  |  |  |  |
| `taxRegistration` |  | partner-taxRegistrationCollection |  |  | [`partner-taxRegistrationCollection`](#partner-taxregistrationcollection) |  |
| `taxRounding` |  | object |  |  |  |  |
| `taxRounding.id` | Internal identifier | string |  |  |  | `DOWN`, `UP`, `OFF` |
| `taxRounding.refName` | Reference Name | string |  |  |  |  |
| `title` | Job Title | string |  |  |  |  |
| `unsubscribe` | Unsubscribe from Campaigns | boolean |  |  |  |  |
| `url` | URL | string |  |  |  |  |
| `vatRegNumber` | VAT Registration No. | string |  |  |  |  |

## partner-addressBook-addressBookAddress

Browser definition `partner-addressBook-addressBookAddress`.

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

## partner-addressBookCollection

Browser definition `partner-addressBookCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | partner-addressBookElement[] |  |  | [`partner-addressBookElement`](#partner-addressbookelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## partner-addressBookElement

Browser definition `partner-addressBookElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `addressBookAddress` |  | partner-addressBook-addressBookAddress |  |  | [`partner-addressBook-addressBookAddress`](#partner-addressbook-addressbookaddress) |  |
| `addressBookAddress_text` | Address | string |  |  |  |  |
| `addressId` | Internal ID | string |  |  |  |  |
| `defaultBilling` | Default Billing | boolean |  |  |  |  |
| `defaultShipping` | Default Shipping | boolean |  |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `internalId` | Internal ID | integer | int64 |  |  |  |
| `label` | Label | string |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## partner-campaignsCollection

Browser definition `partner-campaignsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | partner-campaignsElement[] |  |  | [`partner-campaignsElement`](#partner-campaignselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## partner-campaignsElement

Browser definition `partner-campaignsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## partner-contactRolesCollection

Browser definition `partner-contactRolesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | partner-contactRolesElement[] |  |  | [`partner-contactRolesElement`](#partner-contactroleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## partner-contactRolesElement

Browser definition `partner-contactRolesElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `contact` |  | contact |  |  | [`contact`](contact.md#contact) |  |
| `contactName` | Contact | string |  |  |  |  |
| `email` | Email | string |  |  |  |  |
| `giveAccess` | Access | boolean |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `password` | Password | string |  |  |  |  |
| `passwordConfirm` | Confirm Password | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `role` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |

## partner-subscriptionMessageHistoryCollection

Browser definition `partner-subscriptionMessageHistoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | partner-subscriptionMessageHistoryElement[] |  |  | [`partner-subscriptionMessageHistoryElement`](#partner-subscriptionmessagehistoryelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## partner-subscriptionMessageHistoryElement

Browser definition `partner-subscriptionMessageHistoryElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## partner-subscriptionsCollection

Browser definition `partner-subscriptionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | partner-subscriptionsElement[] |  |  | [`partner-subscriptionsElement`](#partner-subscriptionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## partner-subscriptionsElement

Browser definition `partner-subscriptionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `lastModifiedDate` | Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subscribed` | Subscribed | boolean |  |  |  |  |
| `subscription` |  | campaignSubscription |  |  | [`campaignSubscription`](campaignSubscription.md#campaignsubscription) |  |

## partner-taxRegistrationCollection

Browser definition `partner-taxRegistrationCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | partner-taxRegistrationElement[] |  |  | [`partner-taxRegistrationElement`](#partner-taxregistrationelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## partner-taxRegistrationElement

Browser definition `partner-taxRegistrationElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `address` | Address | string |  |  |  |  |
| `id` | ID | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `nexusCountry` |  | object |  |  |  |  |
| `nexusCountry.id` | Internal identifier | string |  |  |  | `PR`, `PS`, `PT`, `PW`, `PY`, `QA`, `AB`, `AD`, `AE`, `AF`, `AG`, `AI`, `AL`, `AM`, `AN`, `AO`, `AQ`, `AR`, `AS`, `AT`, `RE`, `AU`, `AW`, `AX`, `AZ`, `RO`, `BA`, `BB`, `RS`, `BD`, `BE`, `RU`, `BF`, `BG`, `RW`, `BH`, `BI`, `BJ`, `BL`, `BM`, `BN`, `BO`, `SA`, `BQ`, `SB`, `BR`, `SC`, `BS`, `SD`, `BT`, `SE`, `BV`, `SG`, `BW`, `SH`, `SI`, `BY`, `SJ`, `BZ`, `SK`, `SL`, `SM`, `SN`, `SO`, `CA`, `SR`, `CC`, `SS`, `CD`, `ST`, `CF`, `SV`, `CG`, `CH`, `SX`, `CI`, `SY`, `SZ`, `CK`, `CL`, `CM`, `CN`, `CO`, `CR`, `TC`, `CS`, `TD`, `CU`, `TF`, `CV`, `TG`, `CW`, `TH`, `CX`, `CY`, `TJ`, `CZ`, `TK`, `TL`, `TM`, `TN`, `TO`, `TR`, `TT`, `DE`, `TV`, `TW`, `DJ`, `TZ`, `DK`, `DM`, `DO`, `UA`, `UG`, `DZ`, `UM`, `EA`, `EC`, `US`, `EE`, `EG`, `EH`, `UY`, `UZ`, `VA`, `ER`, `VC`, `ES`, `ET`, `VE`, `VG`, `VI`, `VN`, `VU`, `FI`, `FJ`, `FK`, `FM`, `FO`, `FR`, `WF`, `GA`, `GB`, `WS`, `GD`, `GE`, `GF`, `GG`, `GH`, `GI`, `GL`, `GM`, `GN`, `GP`, `GQ`, `GR`, `GS`, `GT`, `GU`, `GW`, `GY`, `XK`, `HK`, `HM`, `HN`, `HR`, `HT`, `YE`, `HU`, `IC`, `ID`, `YT`, `IE`, `IL`, `IM`, `IN`, `IO`, `ZA`, `IQ`, `IR`, `IS`, `IT`, `ZM`, `JE`, `ZW`, `JM`, `JO`, `JP`, `KE`, `KG`, `KH`, `KI`, `KM`, `KN`, `KP`, `KR`, `KW`, `KY`, `KZ`, `LA`, `LB`, `LC`, `LI`, `LK`, `LR`, `LS`, `LT`, `LU`, `LV`, `LY`, `MA`, `MC`, `MD`, `ME`, `MF`, `MG`, `MH`, `MK`, `ML`, `MM`, `MN`, `MO`, `MP`, `MQ`, `MR`, `MS`, `MT`, `MU`, `MV`, `MW`, `MX`, `MY`, `MZ`, `NA`, `NC`, `NE`, `NF`, `NG`, `NI`, `NL`, `NO`, `NP`, `NR`, `NU`, `NZ`, `OM`, `PA`, `PE`, `PF`, `PG`, `PH`, `PK`, `PL`, `PM`, `PN` |
| `nexusCountry.refName` | Reference Name | string |  |  |  |  |
| `nexusState` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `taxRegistrationNumber` | Tax Reg. Number | string |  |  |  |  |

## partnerCollection

Browser definition `partnerCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | partner[] |  |  | [`partner`](#partner) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## partnerSelectOptions

Browser definition `partnerSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accessRole` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `category` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contact` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contactList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultShippingAddress` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultTaxReg` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `emailPreference` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `globalSubscriptionStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `image` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `parent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxFractionUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxRounding` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

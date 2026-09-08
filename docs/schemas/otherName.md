# Schemas: otherName

Property tables for definitions owned by `otherName`.

Record page: [otherName](../records/otherName.md).

## Index

- [otherName](#othername) — 64 properties
- [otherName-addressBook-addressBookAddress](#othername-addressbook-addressbookaddress) — 18 properties
- [otherName-addressBookCollection](#othername-addressbookcollection) — 6 properties
- [otherName-addressBookElement](#othername-addressbookelement) — 11 properties
- [otherName-campaignsCollection](#othername-campaignscollection) — 6 properties
- [otherName-campaignsElement](#othername-campaignselement) — 2 properties
- [otherName-subscriptionMessageHistoryCollection](#othername-subscriptionmessagehistorycollection) — 6 properties
- [otherName-subscriptionMessageHistoryElement](#othername-subscriptionmessagehistoryelement) — 2 properties
- [otherName-subscriptionsCollection](#othername-subscriptionscollection) — 6 properties
- [otherName-subscriptionsElement](#othername-subscriptionselement) — 5 properties
- [otherName-taxRegistrationCollection](#othername-taxregistrationcollection) — 6 properties
- [otherName-taxRegistrationElement](#othername-taxregistrationelement) — 10 properties
- [otherNameCollection](#othernamecollection) — 6 properties
- [otherNameSelectOptions](#othernameselectoptions) — 14 properties

## otherName

Browser definition `otherName`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountNumber` | Account ID | string |  |  |  |  |
| `addressBook` |  | otherName-addressBookCollection |  |  | [`otherName-addressBookCollection`](#othername-addressbookcollection) |  |
| `altEmail` | Alt. Email | string |  |  |  |  |
| `altName` | Other name | string |  |  |  |  |
| `autoName` | Auto | boolean |  |  |  |  |
| `balance` | Balance | number | double |  |  |  |
| `bcn` | Business Number | string |  |  |  |  |
| `campaigns` |  | otherName-campaignsCollection |  |  | [`otherName-campaignsCollection`](#othername-campaignscollection) |  |
| `category` |  | otherNameCategory |  |  | [`otherNameCategory`](otherNameCategory.md#othernamecategory) |  |
| `comments` | Comments | string |  |  |  |  |
| `companyName` | Company Name | string |  |  |  |  |
| `contact` |  | contact |  |  | [`contact`](contact.md#contact) |  |
| `contactList` |  | contactCollection |  |  | [`contactCollection`](contact.md#contactcollection) |  |
| `creditLimit` | Credit Limit | number | double |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `dateCreated` | Date Created | string | date-time |  |  |  |
| `defaultAddress` | Default Address | string |  |  |  |  |
| `defaultShippingAddress` | Default Shipping Address | string |  |  |  |  |
| `defaultTaxReg` | Default Tax Reg. Number | string |  |  |  |  |
| `email` | Other Name Email | string |  |  |  |  |
| `emailPreference` |  | object |  |  |  |  |
| `emailPreference.id` | Internal identifier | string |  |  |  | `PDF`, `HTML`, `DEFAULT` |
| `emailPreference.refName` | Reference Name | string |  |  |  |  |
| `entityId` | Entity ID | string |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `fax` | Fax | string |  |  |  |  |
| `firstName` | First Name | string |  |  |  |  |
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
| `middleName` | Middle Name | string |  |  |  |  |
| `mobilePhone` | Mobile Phone | string |  |  |  |  |
| `openingBalance` | Opening Balance | number | double |  |  |  |
| `openingBalanceAccount` |  | account |  |  | [`account`](account.md#account) |  |
| `openingBalanceDate` | Opening Balance Date | string | date |  |  |  |
| `phone` | Phone | string |  |  |  |  |
| `phoneticName` | Furigana | string |  |  |  |  |
| `printOnCheckAs` | Print on Check As | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `salutation` | Mr./Ms... | string |  |  |  |  |
| `subscriptionMessageHistory` |  | otherName-subscriptionMessageHistoryCollection |  |  | [`otherName-subscriptionMessageHistoryCollection`](#othername-subscriptionmessagehistorycollection) |  |
| `subscriptions` |  | otherName-subscriptionsCollection |  |  | [`otherName-subscriptionsCollection`](#othername-subscriptionscollection) |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `taxFractionUnit` |  | object |  |  |  |  |
| `taxFractionUnit.id` | Internal identifier | string |  |  |  | `2`, `1`, `0`, `-1`, `-2` |
| `taxFractionUnit.refName` | Reference Name | string |  |  |  |  |
| `taxIdNum` | Tax ID | string |  |  |  |  |
| `taxRegistration` |  | otherName-taxRegistrationCollection |  |  | [`otherName-taxRegistrationCollection`](#othername-taxregistrationcollection) |  |
| `taxRounding` |  | object |  |  |  |  |
| `taxRounding.id` | Internal identifier | string |  |  |  | `DOWN`, `UP`, `OFF` |
| `taxRounding.refName` | Reference Name | string |  |  |  |  |
| `terms` |  | term |  |  | [`term`](term.md#term) |  |
| `title` | Job Title | string |  |  |  |  |
| `unsubscribe` | Unsubscribe from Campaigns | boolean |  |  |  |  |
| `url` | URL | string |  |  |  |  |
| `vatRegNumber` | VAT Registration No. | string |  |  |  |  |

## otherName-addressBook-addressBookAddress

Browser definition `otherName-addressBook-addressBookAddress`.

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

## otherName-addressBookCollection

Browser definition `otherName-addressBookCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | otherName-addressBookElement[] |  |  | [`otherName-addressBookElement`](#othername-addressbookelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## otherName-addressBookElement

Browser definition `otherName-addressBookElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `addressBookAddress` |  | otherName-addressBook-addressBookAddress |  |  | [`otherName-addressBook-addressBookAddress`](#othername-addressbook-addressbookaddress) |  |
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

## otherName-campaignsCollection

Browser definition `otherName-campaignsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | otherName-campaignsElement[] |  |  | [`otherName-campaignsElement`](#othername-campaignselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## otherName-campaignsElement

Browser definition `otherName-campaignsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## otherName-subscriptionMessageHistoryCollection

Browser definition `otherName-subscriptionMessageHistoryCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | otherName-subscriptionMessageHistoryElement[] |  |  | [`otherName-subscriptionMessageHistoryElement`](#othername-subscriptionmessagehistoryelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## otherName-subscriptionMessageHistoryElement

Browser definition `otherName-subscriptionMessageHistoryElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |

## otherName-subscriptionsCollection

Browser definition `otherName-subscriptionsCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | otherName-subscriptionsElement[] |  |  | [`otherName-subscriptionsElement`](#othername-subscriptionselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## otherName-subscriptionsElement

Browser definition `otherName-subscriptionsElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `lastModifiedDate` | Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subscribed` | Subscribed | boolean |  |  |  |  |
| `subscription` |  | campaignSubscription |  |  | [`campaignSubscription`](campaignSubscription.md#campaignsubscription) |  |

## otherName-taxRegistrationCollection

Browser definition `otherName-taxRegistrationCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | otherName-taxRegistrationElement[] |  |  | [`otherName-taxRegistrationElement`](#othername-taxregistrationelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## otherName-taxRegistrationElement

Browser definition `otherName-taxRegistrationElement`.

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

## otherNameCollection

Browser definition `otherNameCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | otherName[] |  |  | [`otherName`](#othername) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## otherNameSelectOptions

Browser definition `otherNameSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `category` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contact` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contactList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultShippingAddress` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `defaultTaxReg` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `emailPreference` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `globalSubscriptionStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `image` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `openingBalanceAccount` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxFractionUnit` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `taxRounding` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `terms` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

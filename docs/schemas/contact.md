# Schemas: contact

Property tables for definitions owned by `contact`.

Record page: [contact](../records/contact.md).

## Index

- [contact](#contact) — 45 properties
- [contact-addressBook-addressBookAddress](#contact-addressbook-addressbookaddress) — 18 properties
- [contact-addressBookCollection](#contact-addressbookcollection) — 6 properties
- [contact-addressBookElement](#contact-addressbookelement) — 11 properties
- [contactCollection](#contactcollection) — 6 properties
- [contactSelectOptions](#contactselectoptions) — 12 properties

## contact

Browser definition `contact`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `addressBook` |  | contact-addressBookCollection |  |  | [`contact-addressBookCollection`](#contact-addressbookcollection) |  |
| `altEmail` | Alt. Email | string |  |  |  |  |
| `assistant` |  | contact |  |  | [`contact`](#contact) |  |
| `assistantPhone` | Assist. Phone | string |  |  |  |  |
| `category` |  | contactCategoryCollection |  |  | [`contactCategoryCollection`](contactCategory.md#contactcategorycollection) |  |
| `comments` | Comments | string |  |  |  |  |
| `company` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `contactCampaignEvent` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `contactSource` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `contactSourceCampaignCategory` |  | campaignCategory |  |  | [`campaignCategory`](campaignCategory.md#campaigncategory) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `dateCreated` | Date Created | string | date-time |  |  |  |
| `defaultAddress` | Default Address | string |  |  |  |  |
| `email` | Email | string |  |  |  |  |
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
| `isInactive` | Contact is Inactive | boolean |  |  |  |  |
| `isPrivate` | Private | boolean |  |  |  |  |
| `lastModifiedDate` | Last Modified Date | string | date-time |  |  |  |
| `lastName` | Last Name | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `middleName` | Middle Name | string |  |  |  |  |
| `mobilePhone` | Mobile Phone | string |  |  |  |  |
| `officePhone` | Office Phone | string |  |  |  |  |
| `owner` |  | integer | int64 |  |  |  |
| `phone` | Main Phone | string |  |  |  |  |
| `phoneticName` | Furigana | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `salutation` | Mr./Ms... | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `supervisor` |  | contact |  |  | [`contact`](#contact) |  |
| `supervisorPhone` | Sup. Phone | string |  |  |  |  |
| `title` | Job Title | string |  |  |  |  |
| `unsubscribe` | Unsubscribe from Campaigns | boolean |  |  |  |  |

## contact-addressBook-addressBookAddress

Browser definition `contact-addressBook-addressBookAddress`.

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

## contact-addressBookCollection

Browser definition `contact-addressBookCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | contact-addressBookElement[] |  |  | [`contact-addressBookElement`](#contact-addressbookelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## contact-addressBookElement

Browser definition `contact-addressBookElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `addressBookAddress` |  | contact-addressBook-addressBookAddress |  |  | [`contact-addressBook-addressBookAddress`](#contact-addressbook-addressbookaddress) |  |
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

## contactCollection

Browser definition `contactCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | contact[] |  |  | [`contact`](#contact) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## contactSelectOptions

Browser definition `contactSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `assistant` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `category` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `company` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contactCampaignEvent` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contactSource` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `contactSourceCampaignCategory` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `emailPreference` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `globalSubscriptionStatus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `image` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `supervisor` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

# Schemas: customerRefund

Property tables for definitions owned by `customerRefund`.

Record page: [customerRefund](../records/customerRefund.md).

## Index

- [customerRefund](#customerrefund) — 67 properties
- [customerRefund-accountingBookDetailCollection](#customerrefund-accountingbookdetailcollection) — 6 properties
- [customerRefund-accountingBookDetailElement](#customerrefund-accountingbookdetailelement) — 7 properties
- [customerRefund-applyCollection](#customerrefund-applycollection) — 6 properties
- [customerRefund-applyElement](#customerrefund-applyelement) — 15 properties
- [customerRefund-depositCollection](#customerrefund-depositcollection) — 6 properties
- [customerRefund-depositElement](#customerrefund-depositelement) — 10 properties
- [customerRefund-payeeAddress](#customerrefund-payeeaddress) — 18 properties
- [customerRefundCollection](#customerrefundcollection) — 6 properties
- [customerRefundSelectOptions](#customerrefundselectoptions) — 23 properties

## customerRefund

Browser definition `customerRefund`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `accountingBookDetail` |  | customerRefund-accountingBookDetailCollection |  |  | [`customerRefund-accountingBookDetailCollection`](#customerrefund-accountingbookdetailcollection) |  |
| `address` | Pay To | string |  |  |  |  |
| `apply` |  | customerRefund-applyCollection |  |  | [`customerRefund-applyCollection`](#customerrefund-applycollection) |  |
| `arAcct` |  | account |  |  | [`account`](account.md#account) |  |
| `balance` | Current Balance | number | double |  |  |  |
| `cardSwipe` | Card Swipe | string |  |  |  |  |
| `cardholderAuthentication` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `checkNumber` | Check # | string |  |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `cleared` | Cleared | boolean |  |  |  |  |
| `clearedDate` | Date Cleared | string | date |  |  |  |
| `consolidateBalance` | Consolidated Balance | number | double |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `customer` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `customerPaymentAuthorization` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `debitKsn` | Debit KSN | string |  |  |  |  |
| `debitPinBlock` | Debit Pin Block | string |  |  |  |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `deposit` |  | customerRefund-depositCollection |  |  | [`customerRefund-depositCollection`](#customerrefund-depositcollection) |  |
| `dynamicDescriptor` | Soft Descriptor | string |  |  |  |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `handlingMode` |  | object |  |  |  |  |
| `handlingMode.id` | Internal identifier | string |  |  |  | `MIMIC`, `PROCESS`, `SAVE_ONLY` |
| `handlingMode.refName` | Reference Name | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `inputReferenceCode` | Input P/N Ref. | string |  |  |  |  |
| `integrationId` | Integration ID | string |  |  |  |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `nexus` |  | nexus |  |  | [`nexus`](nexus.md#nexus) |  |
| `outputAuthCode` | Auth. Code | string |  |  |  |  |
| `outputReferenceCode` | P/N Ref. | string |  |  |  |  |
| `payeeAddress` |  | customerRefund-payeeAddress |  |  | [`customerRefund-payeeAddress`](#customerrefund-payeeaddress) |  |
| `payeeAddressList` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `payeeAddress_text` | Pay To | string |  |  |  |  |
| `paymentCardCsc` | CSC | string |  |  |  |  |
| `paymentDeviceId` | Payment Device ID | string |  |  |  |  |
| `paymentInstrumentLimit` | Payment Instrument Limit | number | double |  |  |  |
| `paymentOperation` |  | object |  |  |  |  |
| `paymentOperation.id` | Internal identifier | string |  |  |  | `CREDIT`, `REFUND` |
| `paymentOperation.refName` | Reference Name | string |  |  |  |  |
| `paymentOption` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `paymentProcessingProfile` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `status` |  | object |  |  |  |  |
| `status.id` | Internal identifier | string |  |  |  | `R`, `V` |
| `status.refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `toBePrinted` | To Be Printed | boolean |  |  |  |  |
| `total` | Refund Amount | number | double |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Check # | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `transactionToRefund` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `voidJournal` |  | journalEntry |  |  | [`journalEntry`](journalEntry.md#journalentry) |  |

## customerRefund-accountingBookDetailCollection

Browser definition `customerRefund-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customerRefund-accountingBookDetailElement[] |  |  | [`customerRefund-accountingBookDetailElement`](#customerrefund-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customerRefund-accountingBookDetailElement

Browser definition `customerRefund-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## customerRefund-applyCollection

Browser definition `customerRefund-applyCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customerRefund-applyElement[] |  |  | [`customerRefund-applyElement`](#customerrefund-applyelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customerRefund-applyElement

Browser definition `customerRefund-applyElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Payment | number | double |  |  |  |
| `apply` | Apply | boolean |  |  |  |  |
| `applyDate` | Date | string | date |  |  |  |
| `createdFrom` | Created From | string |  |  |  |  |
| `currency` | Currency | string |  |  |  |  |
| `doc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `due` | Amt. Due | number | double |  |  |  |
| `job` | Job ID | integer | int64 |  |  |  |
| `jobName` | Subcustomer | string |  |  |  |  |
| `line` | Line Id | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `refNum` | Ref No. | string |  |  |  |  |
| `total` | Orig. Amt. | number | double |  |  |  |
| `type` | Type | string |  |  |  |  |

## customerRefund-depositCollection

Browser definition `customerRefund-depositCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | customerRefund-depositElement[] |  |  | [`customerRefund-depositElement`](#customerrefund-depositelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customerRefund-depositElement

Browser definition `customerRefund-depositElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `amount` | Payment | number | double |  |  |  |
| `apply` | Apply | boolean |  |  |  |  |
| `currencyName` | Currency | string |  |  |  |  |
| `depositDate` | Date | string | date |  |  |  |
| `doc` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `refNum` | Ref No. | string |  |  |  |  |
| `remaining` | Amount Remaining | number | double |  |  |  |
| `total` | Orig. Amt. | number | double |  |  |  |

## customerRefund-payeeAddress

Browser definition `customerRefund-payeeAddress`.

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

## customerRefundCollection

Browser definition `customerRefundCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | customerRefund[] |  |  | [`customerRefund`](#customerrefund) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## customerRefundSelectOptions

Browser definition `customerRefundSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `arAcct` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `cardholderAuthentication` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customer` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customerPaymentAuthorization` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `handlingMode` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `nexus` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `payeeAddressList` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentOperation` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentOption` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `paymentProcessingProfile` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `status` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `transactionToRefund` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `voidJournal` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |

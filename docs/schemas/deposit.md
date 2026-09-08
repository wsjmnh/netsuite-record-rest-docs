# Schemas: deposit

Property tables for definitions owned by `deposit`.

Record page: [deposit](../records/deposit.md).

## Index

- [deposit](#deposit) — 38 properties
- [deposit-accountingBookDetailCollection](#deposit-accountingbookdetailcollection) — 6 properties
- [deposit-accountingBookDetailElement](#deposit-accountingbookdetailelement) — 7 properties
- [deposit-appliedRulesCollection](#deposit-appliedrulescollection) — 6 properties
- [deposit-appliedRulesElement](#deposit-appliedruleselement) — 9 properties
- [deposit-cashbackCollection](#deposit-cashbackcollection) — 6 properties
- [deposit-cashbackElement](#deposit-cashbackelement) — 9 properties
- [deposit-otherCollection](#deposit-othercollection) — 6 properties
- [deposit-otherElement](#deposit-otherelement) — 14 properties
- [deposit-paymentCollection](#deposit-paymentcollection) — 6 properties
- [deposit-paymentElement](#deposit-paymentelement) — 24 properties
- [depositCollection](#depositcollection) — 6 properties
- [depositSelectOptions](#depositselectoptions) — 11 properties

## deposit

Browser definition `deposit`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `accountingBookDetail` |  | deposit-accountingBookDetailCollection |  |  | [`deposit-accountingBookDetailCollection`](#deposit-accountingbookdetailcollection) |  |
| `appliedRules` |  | deposit-appliedRulesCollection |  |  | [`deposit-appliedRulesCollection`](#deposit-appliedrulescollection) |  |
| `cashback` |  | deposit-cashbackCollection |  |  | [`deposit-cashbackCollection`](#deposit-cashbackcollection) |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `cleared` | Cleared | boolean |  |  |  |  |
| `clearedDate` | Date Cleared | string | date |  |  |  |
| `createdDate` | Date Created | string | date-time |  |  |  |
| `creditCardProcessor` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `currencyPrecision` | Currency Precision | integer | int64 |  |  |  |
| `customForm` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReason` |  | nsResource |  |  | [`nsResource`](ns.md#nsresource) |  |
| `deletionReasonMemo` | Deletion Reason Memo | string |  |  |  |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `excludeFromGLNumbering` | Exclude from GL Audit Numbering | boolean |  |  |  |  |
| `externalId` | External ID | string |  |  |  |  |
| `id` | Internal ID | string |  |  |  |  |
| `isBaseCurrency` | Base Currency | boolean |  |  |  |  |
| `lastModifiedDate` | Date Last Modified | string | date-time |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `other` |  | deposit-otherCollection |  |  | [`deposit-otherCollection`](#deposit-othercollection) |  |
| `payment` |  | deposit-paymentCollection |  |  | [`deposit-paymentCollection`](#deposit-paymentcollection) |  |
| `postingPeriod` |  | accountingPeriod |  |  | [`accountingPeriod`](accountingPeriod.md#accountingperiod) |  |
| `prevDate` | Previous Effective Date | string | date |  |  |  |
| `primaryBookBaseCurrency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `subsidiary` |  | subsidiary |  |  | [`subsidiary`](subsidiary.md#subsidiary) |  |
| `toBePrinted` | To Be Printed | boolean |  |  |  |  |
| `total` | Amount | number | double |  |  |  |
| `tranCurrencyName` | Transaction Currency | string |  |  |  |  |
| `tranDate` | Date | string | date |  |  |  |
| `tranId` | Deposit # | string |  |  |  |  |
| `transactionNumber` | Transaction Number | string |  |  |  |  |
| `updateCurrency` | Update Currency | string |  |  |  |  |

## deposit-accountingBookDetailCollection

Browser definition `deposit-accountingBookDetailCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | deposit-accountingBookDetailElement[] |  |  | [`deposit-accountingBookDetailElement`](#deposit-accountingbookdetailelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## deposit-accountingBookDetailElement

Browser definition `deposit-accountingBookDetailElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `accountingBook` |  | accountingBook |  |  | [`accountingBook`](accountingBook.md#accountingbook) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `exchangeRate` | Exchange Rate | number | double |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `revRecOnRevCommitment` | Rev Rec on Rev Commit. | boolean |  |  |  |  |
| `tranIsVsoeBundle` | Transaction Is VSOE Bundle | boolean |  |  |  |  |

## deposit-appliedRulesCollection

Browser definition `deposit-appliedRulesCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | deposit-appliedRulesElement[] |  |  | [`deposit-appliedRulesElement`](#deposit-appliedruleselement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## deposit-appliedRulesElement

Browser definition `deposit-appliedRulesElement`.

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

## deposit-cashbackCollection

Browser definition `deposit-cashbackCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | deposit-cashbackElement[] |  |  | [`deposit-cashbackElement`](#deposit-cashbackelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## deposit-cashbackElement

Browser definition `deposit-cashbackElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `amount` | Amount | number | double |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `line` |  | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |

## deposit-otherCollection

Browser definition `deposit-otherCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | deposit-otherElement[] |  |  | [`deposit-otherElement`](#deposit-otherelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## deposit-otherElement

Browser definition `deposit-otherElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | account |  |  | [`account`](account.md#account) |  |
| `amount` | Amount | number | double |  |  |  |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `line` |  | string |  |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `methCash` |  | string |  |  |  |  |
| `methCheck` |  | string |  |  |  |  |
| `paymentMethod` |  | paymentMethod |  |  | [`paymentMethod`](paymentMethod.md#paymentmethod) |  |
| `refName` | Reference Name | string |  |  |  |  |
| `refNum` | Number | string |  |  |  |  |

## deposit-paymentCollection

Browser definition `deposit-paymentCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` |  | deposit-paymentElement[] |  |  | [`deposit-paymentElement`](#deposit-paymentelement) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## deposit-paymentElement

Browser definition `deposit-paymentElement`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `class` |  | classification |  |  | [`classification`](classification.md#classification) |  |
| `currency` |  | currency |  |  | [`currency`](currency.md#currency) |  |
| `department` |  | department |  |  | [`department`](department.md#department) |  |
| `deposit` | Deposit | boolean |  |  |  |  |
| `docDate` | Date | string | date |  |  |  |
| `docNumber` | Number | string |  |  |  |  |
| `entity` |  | customer |  |  | [`customer`](customer.md#customer) |  |
| `id` | ID | integer | int64 |  |  |  |
| `lineId` | Line Id | integer | int64 |  |  |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `location` |  | location |  |  | [`location`](location.md#location) |  |
| `memo` | Memo | string |  |  |  |  |
| `paymentAmount` | Amount | number | double |  |  |  |
| `paymentMethod` |  | paymentMethod |  |  | [`paymentMethod`](paymentMethod.md#paymentmethod) |  |
| `pmtCurrencyPrecision` | Currency Precision | string |  |  |  |  |
| `pmtMethCash` |  | string |  |  |  |  |
| `pmtMethCheck` |  | string |  |  |  |  |
| `pmtUrl` |  | string |  |  |  |  |
| `refName` | Reference Name | string |  |  |  |  |
| `refNum` | Ref No. | string |  |  |  |  |
| `transactionAmount` | Payment Amount | number | double |  |  |  |
| `type` |  | object |  |  |  |  |
| `type.id` | Internal identifier | string |  |  |  | `VendPymt`, `STaxLiab`, `CustCred`, `ItemShip`, `Check`, `RevContr`, `CustChrg`, `Journal`, `OrdResv`, `RevArrng`, `GLAdj`, `InvReval`, `Opprtnty`, `CustRfnd`, `TrnfrOrd`, `CashRfnd`, `Build`, `Unbuild`, `RevComm`, `SalesOrd`, `Rfq`, `VPrepApp`, `TegPybl`, `Deposit`, `WOIssue`, `FinChrg`, `PurchOrd`, `FftReq`, `StatChng`, `DepAppl`, `ExpRept`, `Wave`, `OwnTrnsf`, `StPickUp`, `NettStlm`, `TegRcvbl`, `WOCompl`, `InvAdjst`, `Transfer`, `Paycheck`, `BalJrnal`, `VendBill`, `YtdAdjst`, `XChgJrnl`, `ItemRcpt`, `PChkJrnl`, `Estimate`, `VPrep`, `SysJrnl`, `Commissn`, `TaxPymt`, `RtnAuth`, `CustInvc`, `WorkOrd`, `FxReval`, `PurchCon`, `BinTrnfr`, `LiaAdjst`, `InvDistr`, `LiabPymt`, `VendRfq`, `RevComRv`, `TaxLiab`, `InvcGrp`, `CustAuth`, `VendAuth`, `InvCount`, `CardRfnd`, `InvWksht`, `VendCred`, `PEJrnl`, `BinWksht`, `Custom`, `CustDep`, `CustPymt`, `WOClose`, `PurchReq`, `InbShip`, `CashSale`, `BlankOrd`, `DeprCust`, `CardChrg`, `InvTrnfr` |
| `type.refName` | Reference Name | string |  |  |  |  |

## depositCollection

Browser definition `depositCollection`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `count` | Count | integer | int64 | read-only |  |  |
| `hasMore` | Has More Results | boolean |  | read-only |  |  |
| `items` | Items | deposit[] |  |  | [`deposit`](#deposit) |  |
| `links` | Links | nsLink[] |  | read-only | [`nsLink`](ns.md#nslink) |  |
| `offset` | Query Offset | integer | int64 | read-only |  |  |
| `totalResults` | Total Results | integer | int64 | read-only |  |  |

## depositSelectOptions

Browser definition `depositSelectOptions`.

| Property | Label | Type | Format | Flags | Ref | Enum |
| --- | --- | --- | --- | --- | --- | --- |
| `account` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `class` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `creditCardProcessor` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `currency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `customForm` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `deletionReason` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `department` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `location` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `postingPeriod` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `primaryBookBaseCurrency` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
| `subsidiary` |  | nsResourceSelectOptions |  |  | [`nsResourceSelectOptions`](ns.md#nsresourceselectoptions) |  |
